## Security Services that GitHub Provides

GitHub is the [largest open source community](https://github.com/open-source) in the world, and we believe that to keep building that community we need to help make it secure. Using code security tooling is nothing new to software development though for many developers it's usually associated with expensive license tags making them difficult to use on open source. What if I told you that many of the tools used by GitHub's largest customers are _free_ on public repos?

//add link to advanced security feature page
At GitHub, we we believe that code security is essential for the open source community to build the software that runs the world. That's why many of GitHub's Advanced Security feature set is FREE for public repos on GitHub.com! Some of these features may be familiar to you, such as Secret Scanning, Code Scanning, and Dependabot. In this post I'll explain more on what those features are and how you as a developer can quickly implement them on your public repos.

### :speak_no_evil: Secret Scanning

Have you ever been working on a project and while testing something locally you had to use a password or API key to a local file? Did you then forget to remove it and then accidentally committed it to your repository? If so, you're not alone. At GitHub, we understand that this is a common mistake and that's why GitHub created Secret Scanning.

[Secret Scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning) is a feature that scans for secrets, such as API keys, passwords, and other sensitive information that shouldn't be in your GitHub repo. When a secret is found, GitHub will notify the repository owner and provide guidance on how to remove the secret wherever it's detected. Secret's might not always show up in just your code, they can also be found in your GitHub issues, pull requests, discussions, and wikis. GitHub Secret Scanning will scan all of these locations to ensure that your repo is secure.

Secret Scanning also has a feature called push protection that can help prevent secrets from being pushed to your repository. When push protection is enabled, GitHub will block the push and notify the repository owner that a secret was found. This can help prevent secrets from being accidentally pushed to your repository (and prevent any embarasing situations like I shared earlier).

All of these Secret Scanning features are enabled by default on public repos on GitHub.com, so getting started is as easy as creating a public repo!

### :lock: Code Scanning

One of the largest challenges today in software development is ensuring that open source software is secure. Many of the building blocks of software are open source, and it's important to ensure that the software you're using is as secure as it can be. To provide solution to this challenge, GitHub built Code Scanning to find, show, and provide soluitions to security vulnerabilities for code that's stored in GitHub.

[Code Scanning](https://docs.github.com/en/code-security/code-scanning/introduction-to-code-scanning/about-code-scanning) is GitHub's tool to perform static code analysis to find security vulnerabilities in your code. Static code analysis is the process of analyzing your code without running it to find potential security vulnerabilities and isn't unique to GitHub. What is unique to GitHub is that Code Scanning is powered by CodeQL, a powerful query language that GitHub built to find security vulnerabilities in code. We can go into more detail on CodeQL in a future post, but for now know that CodeQL is used by many of GitHub's largest customers to secure their code.

The best part about this feature? It's also free on public repos on GitHub.com! This means that you can start using Code Scanning to secure your open source projects today.

### :dependabot: Dependabot

Something that many developers might not think about when writing code is the security of the software that they're using to build projects. Say you're writing some code to make a React Native app and you find an open source library to help put the finishing touches on the app. How do you know that the library you're using is secure? That's where Dependabot comes in.

[Dependabot](https://docs.github.com/en/code-security/dependabot/dependabot-alerts/about-dependabot-alerts) is GitHub's tool to help keep your projects free of any insecure (or out of date) libraries while letting you focus on coding. Depending on the language you're working on, Dependabot will scan supported [dependency files](https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#package-ecosystem) for any outdated or insecure dependencies and create alerts and/or pull requests to assist you in updating them. 

Dependabot is free for all public AND private repos on GitHub.com, so you can start securing your projects today!

### Conclusion

Security is a critical part of software development and GitHub is here to help ensure your code is as secure as possible. With features like Secret Scanning, Code Scanning, and Dependabot, GitHub is providing the tools to help secure what's in open source today and whatever is dreamed up in the future. And the best part? These features are all free on public repos on GitHub.com! 

So what are you waiting for? Start securing your projects today!

Have any questions? Reach out here in the community by asking on this post or by creating a discussion post of your own. We're here to help!

Want to keep reading? More security posts in our community blog and on the GitHub Blog:
- [GitHub Blog: Security](https://github.blog/category/security/)
- [Keeping your GitHub account secure with 2FA Fallbacks](https://github.com/orgs/community/discussions/29814)
- [Account Security Best Practices](https://github.com/orgs/community/discussions/72264)