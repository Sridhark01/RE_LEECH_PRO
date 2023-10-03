# Copy-Master

This is a Telegram Bot written in Python for mirroring files on the Internet to your Google Drive or Telegram.


## ***Variables Description:***

- `UPSTREAM_REPO`: GitLab repository URL, if your repo is private add `https://<deploy_token>:<password>@gitlab.com/<your_username>/<repository_name>
` format. `Str`.
  - **NOTE**: Don't forget to remove '<' and '>'. To generate gitlab Deploy Token. Follow [This](https://docs.gitlab.com/ee/user/project/deploy_tokens/#create-a-deploy-token)
              - Any change in docker you need to deploy/build again with updated repo to take effect. 
              - **No Need to delete .gitignore file or any File**
- `UPSTREAM_BRANCH`: Upstream branch for update. Default is `hk_wzmlx`. `Str`
- `BOT_TOKEN`: Telegram Bot Token that you got from [BotFather](https://t.me/BotFather). `Str`
- `OWNER_ID`: Telegram User ID (not username) of the Owner of the bot. `Int`
- `TELEGRAM_API`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>. `Int`
- `TELEGRAM_HASH`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>. `Str`
- `BASE_URL`: Valid BASE URL where the bot is deployed to use torrent web files selection. Format of URL should be `https://app-name-random_code.herokuapp.com/`, where `app-name` is the name of your heroku app Paste the URL got when the App was Made. `Str`
- `TORRENT_TIMEOUT`: Timeout of dead torrents downloading with qBittorrent and Aria2c in seconds. `Int`
  > Must Add else Bot Crashes! Set to 0 even not Needed
- `DATABASE_URL`: Database URL of MongoDb to store all your files and Vars. Add this will be Helpful. `Str`

---

# Extras

## Bot commands to be set in [@BotFather](https://t.me/BotFather)

```
mirror - or /m1 Mirror
qbmirror - or /qm1 Mirror torrent using qBittorrent
leech - or /l1 Leech
qbleech - or /ql1 Leech torrent using qBittorrent
clone - Copy file/folder to Drive
count - Count file/folder from Drive
ytdl - or /y1 Mirror yt-dlp supported link
ytdlleech - or /yl1 Leech through yt-dlp supported link
usetting - /us1 User settings
bsetting - Bot settings
status - /s1 Get Mirror Status message
btsel - Select files from torrent
rss - Rss menu
list - Search files in Drive
search - Search for torrents with API
cancel - Cancel a task
cancelall - Cancel all tasks
del - Delete file/folder from Drive
log - Get the Bot Log
shell - Run commands in Shell
restart - Restart the Bot
stats - /st1 Bot Usage Stats
ping - /p1 Ping the Bot
help - All cmds with description
```
