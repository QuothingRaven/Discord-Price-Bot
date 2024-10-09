// Copyright (c) 2008 Satoshi Nakamoto
//
// Permission is hereby granted, free of charge, to any person obtaining a copy
// of this software and associated documentation files (the "Software"), to deal
// in the Software without restriction, including without limitation the rights
// to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
// copies of the Software, and to permit persons to whom the Software is
// furnished to do so, subject to the following conditions:
//
// The above copyright notice and this permission notice shall be included in
// all copies or substantial portions of the Software.
//
// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
// IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
// FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
// SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR
// OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
// FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
// IN THE SOFTWARE.

# Discord Price Bot

This Discord bot fetches price data from an API and updates its nickname in all the servers it's a member of to display the fetched price. The bot checks for price updates and changes its nickname every minute.

## Prerequisites

To run this bot, you need to have pip installed.

Inside you terminal run "pip install discord.py requests"

## Setup

1. Clone this repository or download the code.

2. Navigate to the project directory in your terminal and run `npm install` to install the required dependencies.

3. Create a new Discord bot:

   a. Go to the [Discord Developer Portal](https://discord.com/developers/applications).

   b. Click the "New Application" button.

   c. Give your application a name and click "Create".

   d. Navigate to the "Bot" tab on the left side of the page and click "Add Bot".

   e. Copy the bot token by clicking on "Copy" under the "Token" section.

4. Delete the ".sample" part of ".env.sample" file in the project directory with the following content:

   DISCORD_TOKEN=your_bot_token_here

   Replace `your_bot_token_here` with the bot token you copied in step 3e.

5. Invite the bot to your server:

   a. In the Discord Developer Portal, navigate to the "OAuth2" tab.

   b. In the "Scopes" section, select "bot".

   c. In the "Bot Permissions" section, select "Change Nickname".

   d. Copy the generated OAuth2 URL, paste it in your browser, and follow the instructions to add the bot to your server.

## Running the bot

In the project directory, run `python bot.py` to start the bot. It will log in to Discord and start updating its nickname according to the fetched price data.

## License

This project is licensed under the [MIT License](LICENSE).
