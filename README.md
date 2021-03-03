# Twitch-Discord Live Notifications
## A rudimentary AWS lambda function for notifying your discord server when you're live on Twitch
---

This lambda function acts as a webhook reciever for Twitch's EventSub API. Full instructions for usage will be in a blog post soon.

## Requirements

* Python 3.x (Tested on AWS 3.7, AWS 3.8 and Windows 3.9.1)
* Internet connection

## Install

To install dependencies in a manner ready for sending to AWS, run the following:
``` bash
$ pip install --target . -r requirements.txt
```

## Usage

This function is intended to run on AWS Lambda. See the blog post for more information.
Make sure to make a copy of env.example.py, rename it to env.py and fill out the required values:

* `DISCORD_WEBHOOK_URL`: the URL Discord provides for its channel webhook
* `TWITCH_USERNAME`: the twitch username to promote

## Credits

* Some bits stolen from [this gist](https://gist.github.com/Bilka2/5dd2ca2b6e9f3573e0c2defe5d3031b2) from Bilka
* Partially based on Birdie's [Discord webhook guide](https://birdie0.github.io/discord-webhooks-guide/examples/twitch.html#twitch) - Twitch example