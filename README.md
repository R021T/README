# Aaronchettan μLearn
> Discord bot for notifications and accessibility 

[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](#)
[![discord.py 2.2.2](https://img.shields.io/badge/discord.py-2.2.2-blue.svg)](#)

## Basic Uses and Functionality

Aaronchettan is a discord Bot coded in discord.py.

# Table of Contents
- [Python discord Bot](#Discord-bot-for-notifications-and-accessibility )
  - [Basic Uses](#Basic-Uses-and-Functionality)
- [Table of Contents](#Table-of-Contents)
- [Requirements](#Requirements)
  - [How to install discord.py](#discord.py-installation)
  - [How to create Database](#Database-creation)
- [Setup](#Setup)
  - [How to create the .env file](#Creating-the-.env-file)
  - [How to run the bot](#Running-the-bot)
  - [Inviting the bot to the server](#Inviting-the-bot-to-the-server)
- [Commands](#Commands)

## Requirements

This bot requires discord.py 2.2.2, which requires Python 3.11 and MySQL 1.0.3

### discord.py installation
You can get discord.py (and other dependencies) via PyPI:

``` Bash
python3 pip install -r requirements.txt
```

### Database Creation
Please create the database with the code sample provided in the repository given below. 

```
https://github.com/gtech-mulearn/db-scripts
```

## Setup

- Create a discord account, log in, and navigate to the `application page`.
- Assign a name to the application and click on `Create`.
- Head to the `Bot` tab, click on `Add Bot`, and confirm.
- Keep the default settings (check `Public bot` and uncheck `Require OAuth2 Code Grant`)

A discord account has been created for the bot.

### Creating the .env file

- Copy the token given because it will be needed to log into the bot and use it in your server. Please make sure that no one else has access to this token because it gives the owner free access to the bot.

- Copy and paste the `.env.sample` to the new file `.env`
- Add the token to `.env` file in the following manner:

```
BOT_TOKEN = "YOUR_TOKEN_HERE"
```

### Running the bot

- After the above processes, open and run `launcher.py`

### Inviting the bot to the server

- After adding the bot to the server, we need to create an `invite link` for the bot.
- Go to the `OAuth2` tab and select `scopes`.
- Choose `permissions` for the bot according to your requirements (for this bot, selecting `text permissions` is sufficient).
- Next, select the `copy` button above permissions and paste the `URL` in the browser.
- Choose a server for which you have `Manage Server Permissions` and click on `Authorize`.

Your bot has now been added to the server!

## Commands

All commands require an admin role which you can set by using `/admin` (requires administrator permissions on the server). The bot will reply with missing permissions otherwise. Executing a command without any argument will prompt the bot to provide you with instructions on how to use the command effectively. In the following list the default prefix `!` is used, but it can be freely changed in the `config.ini` file.

- `/help` shows this set of commands along with a link to the repository.
- `/new` starts the creation process for a new reaction role message. Check [below](#example) for an example.
- `/admin` adds the mentioned role or role id to the admin list, allowing members with a certain role to use the bot commands. Requires administrator permissions on the server.
- `/rm-admin` removes the mentioned role or role id from the admin list, preventing members with a certain role from using the bot commands. Requires administrator permissions on the server.
- `/adminlist` lists the current admins on the server the command was run in by mentioning them and the current admins from other servers by printing out the role IDs. Requires administrator permissions on the server.
