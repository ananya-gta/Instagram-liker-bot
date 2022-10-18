# Instagram-liker-bot

### What is Required?
- Python 3 (prefer to use latest version available)
- Chrome webdriver (although you can adapt it to any driver supported by Selenium)
- Selenium package

### What is Selenium ?
> Selenium is an open-source automation tool used for testing various web applications against multiple web browsers like Google Chrome, Firefox, Opera, Safari, etc. It remotely controls browser instances and emulate a user’s interaction with the browser.

You can read more about Selenium [here](https://www.selenium.dev/documentation/en/introduction/the_selenium_project_and_tools/#selenium-controls-web-browsers)

### Why not use Instagram API ?

Since IG API is quite restrictive and also to make it more believable I use Selenium to emulate user actions. Fun fact, I had IG bot years ago that used API to like and discover posts, but since then API has been restricted and in order to like posts you need to have a special approval or business account.

### In summary the steps are:

- Open log in page, find username and password fields, fill them in and click log in button
- Pop-up notification arises to ask whether you want to _Turn On Notifications_ or not, the bot clicks on _Not Now_.
- Then another pop-up arises to ask whether you want to save the log in info or not, the bot clicks on _Save Info_.
- Then the bot, opens the post and hit the like button
- We repeat the process
- We either keep bot running forever until we stop it manually or until it hits some predefined condition

