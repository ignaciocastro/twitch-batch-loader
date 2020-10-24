# Twitch Clip Batch Downloader  
![example-gif](https://github.com/amiechen/twitch-batch-loader/blob/master/example.gif)

### Pre-Install:

1) Get a Twitch `Client ID` by registering a twitch app [here](https://dev.twitch.tv/dashboard/apps/create).
Set any name and any category, in "OAuth Redirect URL" write "https://twitchapps.com/tokengen/".
Once finished, copy the `Client ID`. You will need it to run the script.

2) Get a Twitch 'OAuth token' in [twitchapps.com/tokengen](https://twitchapps.com/tokengen).
Paste the Client ID you got earlier, leave "Scopes" blank and click "Connect. 
Accept the app access and copy the `OAuth` token. You will need it to run the script.

2) Install python 3 on your machine if you haven't.

### Usage:

1) Install python packages
```
pip install requests
```

2) Delete the example clips in `clips.txt` and the ones your want. Put each URL on it's own line. No commas or anything like that.

3) Then run the batchloader script. When asked, paste your `Client ID` and your `OAuth token` with the word `Bearer` at the beggining (Example: `Bearer 2gbdx6oar67tqtcmt49t3wpcgycthx`
```
cd twitch-batch-loader
python batchloader.py
```

Voilà! once you see the finished message in your terminal, check the `downloads` folder in this repo and you should see the videos there.
