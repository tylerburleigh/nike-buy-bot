# nike-buy-bot

This is a simple bot using Node.js / puppeteer that buys a Nike shoe when it drops.

# Prerequisites

- Node.js
- git command-line tools
- A text editor (I recommend [Notepad++](https://notepad-plus-plus.org))
- A Nike.com account with a credit card already saved to the account for pre-filling

## Install Node.js

- Install [Node.js (LTS)](https://nodejs.org/en/download)
- Test your Node.js installation: First open a terminal (in Windows, you can do `CTRL + R` then type `cmd` and hit `ENTER`), then type `node -v` and you should see something like `v10.16.0` (the current version as of right now).

## Install git

- Install [git](https://git-scm.com/downloads)
- Test your Node.js installation: First open a terminal (in Windows, you can do `CTRL + R` then type `cmd` and hit `ENTER`), then type `git --version` and you should see something like `git version 2.8.1.windows.1` (the current version as of right now).

# Getting started

1. Clone this repository using git

- Open a terminal (in Windows, you can do `CTRL + R` then type `cmd` and hit `ENTER`)
- Enter the following:

`git clone https://github.com/tylerburleigh/nike-buy-bot.git`

2. Make sure you are in the bot directory within the terminal

`cd nike-buy-bot`

3. Install the Node.js dependencies

`npm install`

4. Using a text editor, edit the `bot.js` file in the bot directory. In this file, look for the section called `Parameters to set`. These are the parameters to change:

- user
- pass
- cv_code
- size
- url
- debug
- buy

5. Run the bot

Once you've configured the bot, you can run it

`npm start`

Ideally, you would run it right around the time of the drop.

# Screenshots

The bot works in a series of 9 "rounds", which include loading the shoe page, finding and clicking the desired shoe size, adding it to the cart, logging into your Nike.com account, and submitting an order.

## Round 1 - Loading the shoe page
![Round 1 - Loading the shoe page](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__1_loaded_1576250190.png)

## Round 2 - Finding/scrolling to the size selectors
![Round 2 - Finding/scrolling to the size selectors](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__2_selectors_1576250192.png)

## Round 3 - Clicking the desired shoe size selector
![Round 3 - Clicking the desired shoe size selector](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__3_size_clicked_1576250193.png)

## Round 4 - Scrolling to the add-to-cart button
![Round 4 - Scrolling to the add-to-cart button](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__4_scroll_to_add_button_1576250195.png)

## Round 5 - Clicking the add-to-cart button
![Round 5 - Clicking the add-to-cart button](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__5_clicked_add_button_1576250196.png)

## Round 6 - Logging in when the login modal appears
![Round 6 - Logging in when the login modal appears](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__6_logged_in_1576250198.png)

## Round 7 - Entering the 3-digit credit card validation
![Round 7 - Entering the 3-digit credit card validation](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__7_entered_cv_1576250203.png)

## Round 8 - Clicking the "Save & Continue" button
![Round 8 - Clicking the "Save & Continue" button](https://raw.githubusercontent.com/tylerburleigh/nike-buy-bot/master/extras/demo_screenshots/bot__8_save_continue_1576250204.png)

## Round 9 - Clicking the "Submit Order" button
(not shown here)
