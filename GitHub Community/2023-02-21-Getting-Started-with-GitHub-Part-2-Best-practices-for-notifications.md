Blog written as part of a series for the GitHub Community Discussion page
https://github.com/orgs/community/discussions/47569

## Getting Started with GitHub Part 2: Best practices for notifications

GitHub is where the world creates, stores, and collaborates on code. In this article, we'll explore how GitHub users can keep track of what they're working on and what interests them, through GitHub notification settings.

### Understanding notifications

#### Types of notifications

There are many functions of GitHub that can send notifications, but only two ways to opt into them: participating and subscribing.

Participation notifications come from events that directly involve something attached to you. These notifications could come from a pull request opened or assigned to you, an issue you opened, or a discussion topic you created. These are a few examples; and a exhaustive list can be found in our [documentation](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/about-notifications#default-subscriptions).

Subscription notifications come from events that you choose to opt into. For example, you can subscribe to an open source repo by watching a repository, subscribing to a specific GitHub issue, or subscribing to security alerts in a repository. More examples can be found [here](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/about-notifications#subscription-options).

To view what kind of notifications you will see from a repository, navigate to the repo root page. At the top right of the page there is a dropdown labeled `Watch`, clicking this will show what kind of notifications you'll receive from this repo. `Participating and @mentions` are a the default setting, `All Activity` can be noisy, and `Ignore` will send you nothing. More on `Custom` notifications can be found [here]([../../../images/Email-notifications.png](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications#configuring-your-watch-settings-for-an-individual-repository)).

![Watching](../../../images/Watching-dropdown.png)

#### GitHub Notification Delivery Options

GitHub can send notifications in three ways: through a browser in GitHub.com, through the Github Mobile app, and through email. As a user of Github, you can choose to receive these notifications in any combination of these options. Documentation on how to customize your notification settings can be found [here](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications#choosing-your-notification-settings).

GitHub notifications have a shared state. If you open a notification sent via email, it will mark a web or mobile notification as 'read' in the browser or mobile app. In the next section we'll talk about how you can update your preferences around notifications.

Where I prefer to view my GitHub notifications is the [notification inbox](https://github.com/notifications). The link to this is in the upper right corner of any GitHub.com page, next to the search bar and your profile picture icon. The notification icon will have a dot over it if you have any notifications!
![Notification Icon](../../../images/Notification-icon.png)

In the inbox you can view all active and viewed notifications. Viewing,filtering, and grouping notifications can all be done on this page. Each notification will tell you what repo it's coming from, along with why you received it, and how long ago it arrived. Notifications can be cleared by selecting the checkbox next to them and marking `Done` to continue receiving updates on this topic, or `Unsubscribe` to clear the notification and no longer receive updates.

For example, say you receive a notification about an Pull Request your GitHub Team was mentioned in for feedback. You are interested in learning more, but don't need to see the notification anymore, so you clear it with `Done`. In another example, you might receive a notification for an Issue but it's not something you're working on or are interested in. You can clear the notification via `Unsubscribe` to no longer see updates on this issue.

### Notification Preferences

No matter how you use GitHub, the easiest way to update preferences is on a Github.com. To get to your notification settings, click on your profile icon in the upper right corner and then click `Settings`. On the left side of the settings page you should see a `Notifications` section, click that to view your settings.

As a first step, follow [this guide](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications) to choose your delivery methods—-if any, for participating and watching notifications.

#### Email Settings

If you decide to enable email notifications, you'll have a few more choices to make. On the left of the page, click `Emails` to update those settings.

When creating a GitHub account, you needed to provide an email, you should see that email here along with any other email addresses you've added to GitHub. More documentation on how these settings work can be found [here](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences), now let's return to the `Notification` settings page.

The first thing you should see on this page is selecting a default email address. Take note that this email address is the same as the primary email address we saw on the `Emails` settings page. The dropdown on this portion of this setting allows you to select any other email address connected to your GitHub account to receive notifications.
![Email Settings](../../../images/Email-notifications.png)

Additionally, you can set up custom routing of email notifications based on each GitHub organization you are a part of. This can be extremely helpful if you want to direct notifications from your work organization to your work email, and notifications of a personal organization to your personal email.

#### Watching Settings

In the next section, you can make two choices about automatic watching of repositories. As we talked about earlier, one of the easiest ways to get notifications is to 'Watch' a repository. 

- Automatically watch repositories
- Automatically watch teams

Both of these settings will automatically set you up to receive notifications. Watch repositories will opt you into notifications if you push code to that repo, and watch teams will opt you in if you are a member of a GitHub Team that is @mentioned in a repository.

#### Subscriptions

We talked earlier about the three places where notifications show up, in this dropdown you can choose to receive notfications on GitHub, email, or both. Note that you don't see the GitHub mobile app here, those notifications will be sent through the 'on GitHub' selection. 

Along with Watching, you can make a choice about how you receive Participating, @mentions, and custom subscriptions. Like watching, GitHub mobile notifications are also driven through the 'on GitHub' selection.

When it comes to how you receive notifications, it's best to have them sent to a space that's easy for you to organize. For some, email is perfect because it allows you to use email filtering to sort information. For others, seeing them in a web browser is great because they are all in one spot and don't clutter and email inbox. Play around with both and see which you prefer!

#### System Notifications

In this section you can make choices about how you receive notifications related to other functions of GitHub. More information on Dependabot alerts settings can be found [here](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications#dependabot-alerts-notification-options). More information on GitHub Actions alert settings can be found [here](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications#github-actions-notification-options).

Thanks for spending time to learn about how GitHub notifications work!
For questions related to GitHub notifications please refer to our documentation as a first step. If you have further questions, reach out to the community! Everyone uses GitHub in their own way and we're happy to help answer your questions.
