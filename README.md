<h1 align="center">Telegram File Stream Bot</h3>
<p align="center">
  <a href="https://github.com/EverythingSuckz/TG-FileStreamBot">
    <img src="https://socialify.git.ci/EverythingSuckz/TG-FileStreamBot/image?description=1&font=Source%20Code%20Pro&forks=1&issues=1&logo=https%3A%2F%2Fwww.flaticon.com%2Fpremium-icon%2Ficons%2Fsvg%2F2321%2F2321089.svg&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" alt="Cover Image" height=400>
  </a>
  <p align="center">
    A Telegram bot to stream files to web
    <br />
    <a href="https://telegram.dog/TG_FileStreamBot"><strong>Telegram Bot »</strong></a>
    <br />
    <a href="https://github.com/EverythingSuckz/TG-FileStreamBot/issues">Report a Bug</a>
    |
    <a href="https://github.com/EverythingSuckz/TG-FileStreamBot/issues">Request Feature</a>
  </p>
</p>

<hr>

<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-this-bot">About this Bot</a>
      <ul>
        <li><a href="#original-repository">Original Repository</a></li>
      </ul>
    </li>
    <li>
      <a href="#how-to-make-your-own">How to make your own</a>
      <ul>
        <li><a href="#deploy-on-heroku">Deploy using Heroku</a></li>
        <li><a href="#host-it-on-vps-or-locally">Run it in a VPS / local</a></li>
      </ul>
    </li>
    <li><a href="#setting-up-things">Setting up things</a></li>
    <ul>
      <li><a href="#mandatory-vars">Mandatory Vars</a></li>
      <li><a href="#optional-vars">Optional Vars</a></li>
    </ul>
    <li><a href="#how-to-use-the-bot">How to use the bot</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#contact-me">Contact me</a></li>
    <li><a href="#credits">Credits</a></li>
  </ol>
</details>

## About This Bot

<p align="center">
    <a herf="https://github.com/EverythingSuckz/TG-FileStreamBot">
        <img src="https://www.flaticon.com/premium-icon/icons/svg/2626/2626281.svg" height="100" width="100" alt="Telegram Logo">
    </a>
</p>
<p align='center'>
    This bot will give you stream links for Telegram files without the need of waiting till the download completes
</p>

### Original Repository

The main working part was taken from [Megatron](https://github.com/eyaadh/megadlbot_oss) and thanks to [eyaadh](https://github.com/eyaadh) for his awesome project.

## How to make your own

Either you could locally host or deploy on [Heroku](https://heroku.com)

### Deploy on Heroku

Press the below button to Fast deply to Heroky

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

then goto the <a href="#mandatory-vars">variables tab</a> for more info on setting up environmental variables.

### Host it on VPS or Locally

```sh
git clone https://github.com/EverythingSuckz/TG-FileStreamBot
cd TG-FileStreamBot
virtualenv -p /usr/bin/python3 venv
. ./venv/bin/activate
pip install -r requirements.txt
python3 -m WebStreamer
```

and to stop the whole bot,
 do <kbd>CTRL</kbd>+<kbd>C</kbd>

## Setting up things

If you're on Heroku, just add these in the Environmental Variables
or if you're Locally hosting, create a file named `.env` in the root directory and add all the variables there.
An example of `.env` file:

```sh
API_ID=452525
API_HASH=esx576f8738x883f3sfzx83
BOT_TOKEN=55838383:yourtbottokenhere
BIN_CHANNEL=-100
PORT=8080
FQDN=yourserverip
```

### Mandatory Vars

`API_ID` : Goto [my.telegram.org](https://my.telegram.org) to obtain this.

`API_HASH` : Goto [my.telegram.org](https://my.telegram.org) to obtain this.

`BOT_TOKEN` : Get the bot token from [@BotFather](https://telegram.dog/BotFather)

`BIN_CHANNEL` : Create a new channel (private/public), add [@missrose_bot](https://telegram.dog/MissRose_bot) as admin to the channel and type /id. Now copy paste the ID into this field.


### Optional Vars

`SLEEP_THRESHOLD` : Set a sleep threshold for flood wait exceptions happening globally in this telegram bot instance, below which any request that raises a flood wait will be automatically invoked again after sleeping for the required amount of time. Flood wait exceptions requiring higher waiting times will be raised. Defaults to 60 seconds.

`WORKERS` : Number of maximum concurrent workers for handling incoming updates. Defaults to `3`

`PORT` : The port that you want your webapp to be listened to. Defaults to `8080`

`WEB_SERVER_BIND_ADDRESS` : Your server bind adress. Defauls to `0.0.0.0`

`FQDN` :  A Fully Qualified Domain Name if present. Defaults to `WEB_SERVER_BIND_ADDRESS`

## How to use the bot

:warning: **Before using the  bot, don't forget to add the bot to the `BIN_CHANNEL` as an admin**
 
`/start` : To check if the bot is alive or not.

To get an instant stream link, just forward any media to the bot and boom, its fast af.

## Contributing

Feel free to contribute to this project if you have any further ideas

## Contact me

[![Telegram Channel](https://img.shields.io/static/v1?label=Join&message=Telegram%20Channel&color=blueviolet&style=for-the-badge&logo=telegram&logoColor=violet)](https://telegram.me/harp_tech)
[![Telegram Group](https://img.shields.io/static/v1?label=Join&message=Telegram%20Group&color=blueviolet&style=for-the-badge&logo=telegram&logoColor=violet)](https://telegram.me/harp_chat)

You can contact either via my [Telegram Chat](https://telegram.me/harp_chat) or you can PM me on [@Anjana_Ma](https://telegram.me/Anjana_Ma)

## Credits

- [EverythingSuckz](https://github.com/EverythingSuckz/TG-FileStreamBot) For his repo
- [eyaadh](https://github.com/eyaadh) for his awesome [Megatron Bot](https://github.com/eyaadh/megadlbot_oss)
- [Dan Tès](https://telegram.dog/haskell) for his [Pyrogram Library](https://github.com/pyrogram/pyrogram)
