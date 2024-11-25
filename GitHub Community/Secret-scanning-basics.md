## Secret Scanning Basics in Open Source

The open source community has built the foundation of what is used by the software world today and here at GitHub one of our highest priorities is to keep that community secure. One of the simplest and most effective ways to keep it secure is removing what we call secrets, things like passwords and API tokens that could be used by bad actors to do things they shouldn't. In this post I'll explain how you can use GitHub's Secret Scanning to help keep your open source projects secure.

### Ok, so secrets are important, but what are they exactly?

Many developers may already know what a secret is, but for those who don't, here's a quick refresher. A secret is a piece of sensetive and important information that should be kept hidden or confidential. This could be anything from a password or API token, to an SSH private key or a SQL connection string. Secrets are important because if they fall into the wrong hands they can be used to do things like impersonate someone, steal data, or even take down a website. In the context of open source projects, secrets can be accidentally leaked in a number of ways like in your code, in a pull request, or in a GitHub issue.

### Now that we know what secrets are, let's talk about secret scanning.

Secret scanning is a feature that GitHub provides for [*free*](https://github.blog/news-insights/product-news/secret-scanning-alerts-are-now-available-and-free-for-all-public-repositories/) to open source to help find and remove secrets that exist on GitHub. When you turn on secret scanning for your repository, GitHub will scan your entire repository for known secret formats and notify you if any are found. This is done using a combination of [regular expressions](https://en.wikipedia.org/wiki/Regular_expression) to find anything that looks like a secret in your repos. If a secret is found, GitHub will notify you in the security tab of your repository and give you guidance on how to remove it.

### That sounds great, how do I turn it on?

Excellent question! For starters, to turn on secret scanning you need to be an admin of the repository. If you'd like to test turning on secret scanning along with this walkthrough, you can create a new *public* repository in your own user space and follow along.

With admin permissions to a repo, you can turn on secret scanning by going to the "Settings" tab of your repository, then clicking on "Code Security" in the left sidebar. From there, you scroll down to see secret scanning, but wait it's already enabled! GitHub recenly announced that for all new public repositories, [secret scanning is automatically enabled](https://github.blog/changelog/2024-02-14-secret-scannings-push-protection-will-soon-be-enabled-for-all-free-accounts-on-github/). If you have an older repository, you can turn on secret scanning it by clicking on the "Enable" button in the secret scanning section of the page.

When it comes to enterprise and organization permissions there are  settings to automatically turn on Secret Scanning for private and internal repositories when they are created. These features are built into GitHub Advanced Security, which is a paid feature for GitHub Enterprise Cloud and GitHub Enterprise Server. 

### Great, now that we've turned on secret scanning, where does GitHub scan for secrets?

You are full of great questions today! Secret Scanning searches for secrets in a number of places on GitHub, including the code in your repository, pull requests, and issues. Secret Scanning even searches the comments, descriptions, and titles of your issues and pull requests. This means that if a secret gets accidentally pushed to your reposotiry or if it gets added to a pull request comment as part of a code review, GitHub will find it and let you know about it. 

It's also important to know what exaclty GitHub is scanning for so you know what could be found. GitHub maintains a list of [known secret formats](https://docs.github.com/en/code-security/secret-scanning/introduction/supported-secret-scanning-patterns) that we scans for, which includes things like AWS keys, Google Cloud keys, and our own GitHub API tokens. This list is constantly being updated as new secret formats are discovered and as GitHub's scanning capabilities improve.

### Oh no, a secret was found in my repository! What should I do?

Don't panic, we can learn from what has happened to other leaked secrets take action to fix this. First, you should assume the secret has already been compromised and take steps to revoke it, especially if the secret is still being used. This could mean regenerating an API token, creating a new SSH key, or changing a password. Once you've done that, you can remove the secret from your repository. 

The removal process depends on where the secret was found. 
- If the secret was found in code, then you need to follow a code cleanup process to remove the secret from git history. Simply deleting the secret with the newest commit doesn't remove the secret from past commits. There are two processes to clean up git history, both of which we explain how to do on our [doc site](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository). 
- If the secret was found in an issue or comment, you can [edit the issue or comment](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/editing-an-issue) to remove the secret. Keep in mind this does not remove the commit from the issue history so you should still rotate the secret.

### Phew! Now I know where GitHub scans for secrets, but how should I protect them?

Another great question! There are a number of best practices that you can follow to protect your secrets, some of them involve using GitHub's own features. One of the most common ways secrets get leaked is by hardcoding them into your code. To prevent this, you can use GitHub Actions to [store your secrets](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions) as encrypted environment variables and then use them in your workflows. This way, your secrets are never exposed in your code and are only available to your workflows at runtime.

Other great ways to protect secrets include using password management tools to hold account credentials, storing your secrets in a vault, and using two-factor authentication to protect your accounts. When it comes to securing you GitHub account, I've written a [best practices guide](https://github.com/orgs/community/discussions/72264) that you can check out for more information.

### That was helpful! Is there more I should learn about secret scanning?

This blog is only a high level first step on secret scanning. If you'd like to learn more we have public [documentation](https://docs.github.com/en/code-security/secret-scanning/introduction/about-secret-scanning) on our doc site. Addtionaly, please use the community space to find answers ask more (great) questions and share your experiences with other developers around secret scanning. When we all work together to keep our secrets safe, we can build a more secure open source community.

Happy coding!