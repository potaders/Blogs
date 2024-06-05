Blog written as part of a series for the GitHub Community Discussion page
https://github.com/orgs/community/discussions/72264

## Getting Started with GitHub Part 3: Account Security Best Practices

**[Starting in 2023, all GitHub.com accounts must have 2FA enabled](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/about-mandatory-two-factor-authentication)**

Online communities will always be subjected to malicious activity, and GitHub is no exception. It's important to take the necessary steps to protect your account and its content from hackers and other nafarious individuals. In this article, we'll cover some of the best practices you can follow to help keep your account secure.

## Passwords

The first and arguably the most important step to securing your Github account is using a strong password. There are many factors that can go into creating a great password, but the most important thing to remember is to make sure your passwords are strong and unique. Using the same email/username and password combination for everything online can mean it only takes one compromised service to put all of your accounts in jeopardy. For mor information on how to create a strong password, I recommend reviewing [our guide](https://help.github.com/articles/creating-a-strong-password/) on how to get started.

At GitHub, we believe the best way to generate and keep track of all your passwords is to use a password manager. These applications make generating strong passwords extremely simple and can be and can help you avoid the issue of reusing username/password combinations. While GitHub doesn't officially any specific password manager, many people in the communtiy [1Password](https://1password.com/) or [BitWarden](https://bitwarden.com/). There are many password manager options out there, I always suggest that you do some research and find the one that works best for you.

Additionally, keep in mind that a password manager is only as secure as the password you use to secure it, so you'll want to be sure to apply the same principles here: make your master password unique and hard to guess. [Using a mnemonic](https://xkcd.com/936/) is a great way to avoid avoid forgetting the password you create for your password manager.

## Two-factor authentication (2FA)

Two-factor authentication is a great way to add an extra layer of security to your GitHub account. It requires you to provide a second piece of information to authenticate, rather than just your password. 

The idea behind 2FA can be often be explained as "something you know" and "something you have". For example, when using an ATM you typically need both your bank card (something you have) and your PIN (something you know) to withdraw cash. Without both of these things, you wouldn't be able to log into your account at all. This is the same idea behind 2FA, but instead of a bank card and PIN, you'll use your password and a second piece of information to log in to your account.

With 2FA enabled, if someone were to get ahold of your password, they would still need access to another piece of information (like your phone or another device) to log in to your GitHub account. GitHub offers a few different methods of two-factor authentication, so you can choose the one that works best for you. 

### Primary methods

Now that you have a better understanding of what 2FA is, let's take a look at the primary methods of 2FA that GitHub offers.

**SMS-based Authentication**

When authenticating via SMS, GitHub will generate an authentication code for you every time you provide a valid password at login. This code is then sent to the phone number associated with your account; providing it when prompted will complete the sign-in process, allowing you to login to the account and access its content.

SMS based authentication has its benefits. You only need access to a cellular network in order to recieve the codes we send. However, if you're in an area that provides little to no cellular coverage, this could prevent you from being able to access your account. Additionaly, if for some reason you have to change/update phone numbers, you may lose access to your account.

Learn more about enabling SMS-based authentication for your GitHub account [here](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication#configuring-two-factor-authentication-using-text-messages).

**TOTP Applications**

TOTP (Time-based One-Time Password) applications are another great way to add an extra layer of security to your GitHub account. These applications generate a new authentication code every 30 seconds, which you can then use to authenticate with your GitHub account. This means that even if someone were to get ahold of your password, they would still need access to your phone or other device with the TOTP app installed to log in to your GitHub account.

GitHub supports the use of any cloud-based TOTP apps such as Duo, Google Authenticator, Microsoft Authenticator, and Authy. While using these apps is a more secure way to protect your GitHub account, it does create some different problems when compared to SMS-based authentication. For example, if you regularly upgrade or change phones, you'll need to take extra care to ensure you have a fallback authentication method configured. By not doing this, you could be unable to access your GitHub account to configure a new TOTP device.

If you're interested in configuring two-factor authentication using a TOTP application, we have a guide that can walk you through this [here](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication#configuring-two-factor-authentication-using-a-totp-app).

### Secondary and fallback methods

While primary 2FA methods are required to be configured on your account, secondary and fallback methods are optional. These are intended provide alternative login styles and to be used as a backup in the event that you lose access to your primary method of authentication.

**Secondary methods**

Secondary methods are used to provide an alternative method of 2FA to your GitHub account. All of the methods listed below require you to already have a primary method of 2FA configured on your account. I'm not going to go into great detail on these methods, to learn more here are some links to configure the secondary methods that GitHub offers:

- [Passkey authentication](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication#configuring-two-factor-authentication-using-a-passkey) - Passkeys come in the form of fingerprint sensors or facial recognition. More info on Passkeys can be found [here](https://docs.github.com/en/authentication/authenticating-with-a-passkey/about-passkeys).
- [Security key authentication](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication#configuring-two-factor-authentication-using-a-security-key) - Security keys often come in the form of a physical device like a [YubiKey](https://www.yubico.com/products/).
- [GitHub Mobile App](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication#configuring-two-factor-authentication-using-github-mobile) - Our very on [GitHub Mobile App](https://github.com/mobile)!

**Fallback methods**

Fallback methods are used when you lose access to your primary method of authentication. For example, if you normally authenticate with a TOTP application, but lose access to your phone, you can use a fallback method to authenticate with your GitHub account. I cover a few great benefits of using fallback methods in another blog post [here](https://github.com/orgs/community/discussions/29814).

**Recovery codes**

These set of codes are automatically generated for you when you enable 2FA on GitHub and are designed to be used as a 'break-glass in case of emergency' method of logging back into your GitHub account. It is *incredibly* important to keep these codes in a very secure location as they can be used to bypass all other methods of 2FA on your account. This is something that you should remember to do every time you set up a new 2FA configuration on any account, not just GitHub. 

If you do have 2FA enabled and don't know where your codes are or don't have access to them anymore, I suggest pausing right now and going to [this page](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication-recovery-methods#generating-a-new-set-of-recovery-codes) to follow our documentation to download a new set of recoery codes. Once you have the new codes (or find your existing codes), I suggest storing them in a secure location like a password manager or print them out and store them in a safe place.

## Other Security Considerations

### SSH keys

SSH keys are typically used to authenticate with GitHub when using Git over SSH. While they are not categorized as a form of 2FA, they are essential to how many of the developers on GitHub use our services to push and pull code. If you're interested in learning more about SSH keys at GitHub, we have a guide that can be found in [our documentation](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh).

To get started with using and securing SSH keys on GitHub, follow the steps in our guide [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

#### Personal access tokens (PAT)

Personal access tokens are a one of the most flexible ways to connect to and use GitHub. In many functions on GitHub they can be used in like a password and can be revoked by you at any time. This means that if you're using a PAT and you lose access to it, you can simply revoke it and generate a new one. 

Even though a PAT can be revoked at any time, it should still be treated like a secret and not shared or stored in any public location, like in a GitHub repository. You can (and should) create PATs that will automatically expire after a certain amount of time. this is a great way to ensure that you don't accidentally leave a PAT laying around that could be used to access your account.

### Securing for success!

Thank you for taking the time to review some best practices when securing your GitHub account. Now that you know more, please take some time to review your existing GitHub account settings and make sure that you have the appropriate security measures in place to protect your account.

[https://github.com/settings/security](https://github.com/settings/security)

If you have any questions about the account security topics covered in this article, please reach out to our fantastic support team by going to [support.github.com](https://support.github.com/).

Links to part 1 and part 2 of this series can be found below:

- [Part 1](https://github.com/orgs/community/discussions/39082)
- [Part 2](https://github.com/orgs/community/discussions/47569)