# Ignition
Ignition is a Discord bot made to manage remote game servers via Discord bot commands.

# Getting Started

Make sure you have an available bot account. You can configure one here-
https://discord.com/developers/applications

If you're unfamiliar with setting up a Discord bot account, I'd Google a guide! It'll be important to set bot permissions so it can see server commands.

You're going to want your Gateway Intents to look something like this.

![image](https://user-images.githubusercontent.com/68837573/228999275-dbb92bfe-4b2e-430a-acf6-a4f8eec50a7b.png)

Download the .zip to any directory, and unzip it!

# Setting Up

Put your bot's token in the ".env" file.

By default, the "settings.json" file looks like this.
```
{   "Admin ID List": [111111111111111111, 222222222222222222],
    "Command Prefix": "!",
    "nickname": [
        "path from main drive",
        "custom argument to launch instead of from path"
    ],
    "Quake3": [
        "C:/Users/SampleUser/Documents/Q3-152-beta/Q3/cnq3-server-x64.exe",
        "cd C:/Users/SampleUser/Documents/Q3-152-beta/Q3 && start /B start.bat"
    ],
    "Chrome": [
        "C:/Program Files/Google/Chrome/Application/chrome.exe",
        ""
    ]
}
```
I've left a few sample configurations for you to reference. :)

This is where you'll store the application nicknames (used in commands), your default prefix, the UIDs of Discord members you want to be able to start and stop applications, and any custom arguments/CLI executions. In your custom arguments, remember to mind your working directory!

And that's it! Start the bot by running bot.exe!

# Commands
```
{settings["Command Prefix"]}start [servername]      - Start a server.
{settings["Command Prefix"]}restart [servername]    - Restart a server.
{settings["Command Prefix"]}stop [servername]       - Stop a server.
{settings["Command Prefix"]}stopall                 - Stop all active servers.
{settings["Command Prefix"]}check [servername]      - Check status of a specific server.
{settings["Command Prefix"]}help                    - Command list and status.
```

