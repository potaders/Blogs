Blog written as part of a series for the GitHub Community Discussion page
https://github.com/orgs/community/discussions/39082

## Getting Started with GitHub Part 1: Best practices for setting up your GitHub account

### Creating a username

Welcome to GitHub! Thank you for starting your journey on the largest developer community in the world!

The first thing you need to do when using GitHub is create an account. Whether you're working in open source projects, working with friends on a school project, or just exploring a new tool that you overheard some people talking about at work, a GitHub account grants you basic access to the platform.

To create your account, you'll need to have 3 things:

- A unique username, or handle :tada:
- An email address :mailbox:
- A password :lock:

### Your handle

At GitHub, your handle is super important. It is a public reference that can be traced back to all public (and sometimes private) things you do on GitHub. That can seem daunting, but it can also be fun! Handles at GitHub are an individual thing, no 2 are exactly the same, so take the time to decide on something that shows off the amazing person that you are. Selecting a handle can be a hard decision, thats where we can help!

#### Be yourself

As stated above, handles are highly visible, so it only makes sense that they should show who you are as individual or who you want to be perceived as. Please keep in mind that a handle is also something that you should feel comfortable being public. Handles are often added to resumes so having a handle that is respectful may help recruiters feel comfortable about bringing in a candidate for a job interview. 

Handles also area a great opportunity to show off more about yourself than your development. Maybe you have a love of a certain type of music, maybe you connect with a certain comic book character, or maybe you're an animal lover, etc. Keep in mind that trends sometimes pass, so creating a handle that is associated with a specific topic could age poorly.

Quick note: GitHub handles may only contain 39 alphanumeric characters and a hyphen (ex. `good-handle`). Hyphens can only be used once in a handle (ex. `not-allowed-handle`) and cannot be at the beginning or end of the handle (ex. `-notallowed-`). GitHub is a community for everyone, please consider reading [this page](https://docs.github.com/en/site-policy/acceptable-use-policies/github-hate-speech-and-discrimination) as well before creating a handle.

**Attention**: It is technically possible to change your GitHub handle, doing so will not update any references to your past handle. To learn more, review documentation found [here](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-personal-account-settings/changing-your-github-username).

At the end of the day, your GitHub handle will become your calling card when interacting with all things GitHub. Other GitHub users will use it as a reference when asking you questions, assiging you tasks, or looking at your public contributions. More info [here](https://docs.github.com/en/site-policy/other-site-policies/github-username-policy).

### Creating a repository

Now that you have a handle, you can now create a repository. You can create repositories in a few places, but the easiest place to start is in your personal org. In the upper right corner of the GitHub.com, you will see a plus sign. Clicking on that will provide a prompt allowing you to create a new reposoitory. 

Repo creation screen should look something like this: 
![Repo Screenshot](../../../images/repo-create-screenshot.png)

When creating a repository, the only required detail is the name of the repository. Repository names cannot have spaces, so any space you leave in your name will automatically be filled with dashes `-`. Optionally, you can include a description which can be used to help provide details about what is in the repository. For example, if you're working on a mobile app, you could name the repository "My-cool-app" and provide a description of "My mobile app writen in React Native". This makes the repository much more approachable in the event that you want to share your cool app with the world!

#### Public or private repositories?

When creating a repository you have the option of setting the repository as public or private. Public repositories are exaclty as they sound, public! They are open for the world to see and can be viewed by anyone on GitHub. This is a good route if you're looking to share your work and potentially get public feedback and contributions. In contrast to public, private repositories are not visible to anyone other than you. With private repositores you also have the power to invite in other GitHub users to view and collaborate on your code.

The default choice when creating a repository is private, though it's not always the best choice. Say you're working on a new React Native app and you make a really slick menu bar. If your repository is public, then anyone who finds it would be able to use your code and improve their apps. By keeping your project public, anyone who finds your project could help you make improvements to your code through Issues and Pull Requests.

#### Initialize with a README.md?

The final step to creating a repositroy is deciding whether to initiate it with a README. At GitHub, nearly all of our repositories have a README files and they serve a very important purpose. Creating your repository with a README is an excellent choice if you are starting from scratch and can help save time by avoiding the need to import an existing git project. 

For those who are planning to import an existing git project, it is best to avoid selecting the 'initiate with README' checkbox. This will help you avoid conflicts in your git history when pushing the contents of your existing project into your new GitHub repository.

As stated above, at GitHub, the README file serves a very important purpose. The README(.md) file is extra special because it will be automatically shown as the first thing you see when viewing your GitHub repository from a web browser. Think of the README file as a guide to all of the things in your repository; it's the place where you get to share all of the important information about your repository and show others how to use your code. Visitors and contributors to your repository should be able to read through your project's README file and understand what your project does, who to contact for questions, how they can use it, and how to contribute.

README files are writen in language called Markdown, which supports showing many varieties of information including images, links, GIFs, emojis, tables, and many others! While Markdown cheatsheets can be found all over the internet, GitHub does have some helpful docs that can asist you in geting you started [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

To paint a picture, let's take a look at a README file for a very popular open source tool on GitHub, [Visual Studio Code](https://github.com/microsoft/vscode). The first thing you may notice in the README are some helpful 'badges'. These badges can be used to show all sorts of helpful information, in this example, VS Code has chosen to show issue counts and open bugs. Other popular badges include showing information about build status from a CI (Continuous Integration) tool, chat ops connection like Slack, or test coverage status. Next, as we move down the VS Code README, we see more information about the product, how to make contributions, how to provide feedback, and additional information about licensing, building, and a code of conduct. Not all of this information is needed in your README, but it can be very helpful to get an idea about what you'd like to share about your project.

The README files are a great starting point to your project, but they are far from the final step. You should expect your README file to change as your project changes, so when your React app grows to include some new features, you should expect your README to grow too!

### Welcome to GitHub!

That's all for now; welcome to GitHub. We are overjoyed that you have joined the largest developer community in the world. From amazing handle, to fresh code, we are excited build with you from here, together!
