# Website Reminder - Correct Login Option

By Weng Fei Fung. You ever login on some website that asks if you want to use your Facebook, Google (and you might have several Google accounts), Amazon, or email or username? With so many login options on some websites, you may forget which one you signed up with. This TamperMonkey snippet lets you know the correct login option at the bottom right whenever you visit such websites.

## TamperMonkey

You need to install the extension TamperMonkey for my snippets to work. Go ahead and google TamperMonkey for your web browser.

## How to use

Inside the logins folder https://github.com/Siphon880gh/website-reminder-correct-login-option/tree/master/logins are snippets for websites that you use Facebook, Google, etc to login.

### Editing the snippets

If you have a website like medium.com that offers multiple choices of logging in and you signed up with Facebook, then you want to install the Facebook snippet from the login folder and make sure the text has https://www.medium.com

```
// @match        https://medium.com/
```

For additional websites that use Facebook login, you add more match lines like this:

```
// @match        https://www.website1.com/
// @match        https://www.website2.com/
```

Make sure the https or http matches. Some websites will get rid of the "www" when you visit them. The URL needs to match exactly what you see on the address bar.


If you have a website that offers those multiple social network logins but you signed up with your own username or email, there's a not-social-media.txt snippet that reminds you not to login with a social media. You wouldn't want to end up with multiple accounts because some websites equate logging in to a social media as creating an account.

### Adding the snippets

After you add the websites to the snippet, to actually install it, click the TamperMonkey icon on your web browser => Dashboard => Plus icon.

Copy and paste the snippet to there. Then File => Save. Now whenever you visit the URLs you added, then the website reminder appears at the bottom. You repeat this process for other Login types.