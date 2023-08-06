# Aaronchettan μLearn
> Discord bot for notifications and accessibility

[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](#)
[![discord.py 2.2.2](https://img.shields.io/badge/discord.py-2.2.2-blue.svg)](#)
[![mysql 1.0.3](https://img.shields.io/badge/mysql-1.0.3-blue.svg)](#)

## Basic Uses and Functionality

Aaronchettan is a discord Bot coded in discord.py, which is used to moderate our discord server and for karma automation. 

# Table of Contents
- [Setup](#setup)
- [Installation](#install)
  - [How to create the .env file](#env-file)
  - [How to run the bot](#bot-run)
- [Inviting the bot to the server](#bot-invite)
- [Commit Types](commit)
- [Commands](#commands)
- [Contributing](#contributing)
- [Licensing](#licensing)


<a name="setup"/>

## Setup

- Create a discord account, log in, and navigate to the `application page`.
- Assign a name to the application and click on `Create`.
- Head to the `Bot` tab, click `Add Bot`, and confirm.
- Keep the default settings (check `Public bot` and uncheck `Require OAuth2 Code Grant`)

A discord account is thus created for the bot.

<a name="install"/>

## Installation

```bash
# Fork and Clone the repository
git clone https://github.com/@github_username/aaronchettan.git

# Enter into the directory
cd aaronchettan/

# Install the dependencies
python3 pip install -r requirements.txt

```

Please create the database with the code sample in [Database Script](https://github.com/gtech-mulearn/db-scripts/blob/main/latest.sql). 

<a name="env-file"/>

### Creating the .env file

- Copy the token given because it will be needed to log into the bot and use it in your server. Please make sure that no one else has access to this token because it gives the owner free access to the bot.

- Copy and paste the `.env.sample` to the new file `.env`
- Add the token to the `.env` file in the following manner:

```python
BOT_TOKEN = "YOUR_TOKEN_HERE"
```
<a name="bot-run"/>

### Running the bot

- After the above processes, open and run `launcher.py`

<a name="bot-invite"/>

## Inviting the bot to the server

- After adding the bot to the server, we need to create an `invite link` for the bot.
- Go to the `OAuth2` tab and select `scopes`.
- Choose `permissions` for the bot according to your requirements (for this bot, selecting `text permissions` is sufficient).
- Next, select the `copy` button above permissions and paste the `URL` in the browser.
- Choose a server for which you have `Manage Server Permissions` and click on `Authorize`.

The bot is added to the server successfully.

<a name="commit"/>

## Commit message types
```python
- feat: (adds valuable new features or improvements that directly benefit and engage users.)
  #feat(column): Added new feature
 
- fix: ( resolve user-related issues, improving the software's reliability and providing a smoother user experience.)
  #fix(case): Fixed case sensitivity issue in search functionality for accurate results.

- docs: (making changes or updates to the documentation for better clarity and understanding.)
  #docs(readme): Updated README file with installation instructions and usage examples.

- style: ( focus on improving code appearance, such as formatting and fixing missing semicolons, without affecting functionality.)
  #style(format): Corrected indentation and added missing semicolons for consistent code style.

- refactor: (modifying the production code, such as renaming variables, to improve its structure and maintainability.)
  #refactor(variables): Renamed variables for improved code clarity and maintainability.

- test: (adding tests that were missing and improving existing tests, without changing the production code.)
  #test(login): Added tests for user login functionality and refactored existing login tests.

- chore: (updating build tasks and other non-production code aspects, without changing the actual software.)
  #chore(grunt): Updated Grunt tasks for better task automation and build process efficiency.
```
  
<a name="commands"/>

## Commands

Provided below is a list of basic commands to try out to ensure their functionality regarding the corresponding action to be performed by the bot.

```python
# For any assistance or support from the µLearn Team
/support-ticket
```
```python
# To fetch your µid in case you don't remember
/get-muid
```
```python
# To edit your profile to integrate other services like GitHub with your ATFG µLearn profile
/edit-profile
```
```python
# To check your profile and rank based on your activities on the μLearn platform
/rank
```

## Contributing

You are welcome to contribute by submitting a Pull Request to the repository , see the [CONTRIBUTING.md](CONTRIBUTING.md) file for details.
