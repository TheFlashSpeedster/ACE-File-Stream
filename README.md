# ACE - File Stream

`This bot will give you stream links for Telegram files without the need of waiting till the download completes`

``` 
💥 Superfast download and stream links.
💥 No ads in generated links.
💥 Superfast interface.
💥 Along with the links you also get file information like name,size ,etc.
💥 Updates channel Support.
💥 Mongodb database support for broadcasting.
```

### Channel Support
`Bot also Supports with Channels. Just add bot Channel as Admin. If any new file comes in Channel it will edit it with Get Download Link Button.` </details>

## Commands
```
start - Start the Bot
help  -  How to Use
status  - Statistics
broadcast - Broadcast message to all users
```
## Deploy to Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/TheFlashSpeedster/ACE-File-Stream)

## Deploy on VPS
</summary>


```py
git clone https://github.com/TheFlashSpeedster/ACE-File-Stream
cd ACE-File-Stream
virtualenv -p /usr/bin/python3 venv
. ./venv/bin/activate
pip install -r requirements.txt
python3 -m Adarsh
```
• To stop the bot: <kbd>CTRL</kbd>+<kbd>C</kbd>

## Setting up things

If you're on Heroku just add these in the Environmental Variables
or if you're Locally hosting, create a file named `.env` in the root directory and add all the variables there.
An example of `.env` file:

```py
DATABASE_URL=  Get this from mongodb.com
PORT=8080
API_ID= Get from my.telegram.org
NO_PORT=False
BOT_TOKEN= Get from botfather
OWNER_ID= your owner id 
API_HASH= Get from my.telegram.org
UPDATES_CHANNEL= Enter Force sub channel username without @ if any  else set value to None
BIN_CHANNEL=-100
SESSION_NAME=Codexmania
HAS_SSL=True
FQDN= Enter Custom domain if any or server ip
```
 <b>Vars and Details :</b>
`API_ID` : Goto [my.telegram.org](https://my.telegram.org) to obtain this.

`API_HASH` : Goto [my.telegram.org](https://my.telegram.org) to obtain this.

`BOT_TOKEN` : Get the bot token from [@BotFather](https://telegram.dog/BotFather)

`BIN_CHANNEL` : Create a new channel (private/public), add [@missrose_bot](https://telegram.dog/MissRose_bot) as admin to the channel and type /id. Now copy paste the ID into this field.

`OWNER_ID` : Your Telegram User ID
  
`OWNER_USERNAME` : Your telegram username to be displayed in bot  . make one in you dont have.

`DATABASE_URL` : MongoDB URI for saving User IDs when they first Start the Bot. We will use that for Broadcasting to them. I will try to add more features related with Database. If you need help to get the URI you can ask in [Telegram](https://t.me/codexmania).

 Optional Vars

`UPDATES_CHANNEL` : Put a Public Channel Username, so every user have to Join that channel to use the bot. Must add bot to channel as Admin to work properly.

`BANNED_CHANNELS` : Put IDs of Banned Channels where bot will not work. You can add multiple IDs & separate with <kbd>Space</kbd>.

`SLEEP_THRESHOLD` : Set a sleep threshold for flood wait exceptions happening globally in this telegram bot instance, below which any request that raises a flood wait will be automatically invoked again after sleeping for the required amount of time. Flood wait exceptions requiring higher waiting times will be raised. Defaults to 60 seconds.

`WORKERS` : Number of maximum concurrent workers for handling incoming updates. Defaults to `3`

`PORT` : The port that you want your webapp to be listened to. Defaults to `8080`

`WEB_SERVER_BIND_ADDRESS` : Your server bind adress. Defauls to `0.0.0.0`

`NO_PORT` : If you don't want your port to be displayed. You should point your `PORT` to `80` (http) or `443` (https) for the links to work. Ignore this if you're on Heroku.

`FQDN` :  A Fully Qualified Domain Name if present. Defaults to `WEB_SERVER_BIND_ADDRESS` </details>
