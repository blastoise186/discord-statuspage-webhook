# Discord Status Webhook
## What is it?
This script will send a message to your server when the [Discord status page](https://status.discordapp.com/) is updated

## Setup
1. Clone this repository
`git clone https://github.com/Benricheson101/discord-statuspage-webhook.git`
2. Install the dependencies
`npm install`
3. Compile typescript
`npm run build`
4. Setup your config (see below)
5. Make a blank json file: `src/webhook/latest.json` 
6. Start the script
`npm run start`

## Config
Make `src/config.js` and configure the following:
```js
module.exports.oauth = {
	client_id: "",
	client_secret: "",
	grant_type: "authorization_code",
	redirect_uri: "",
	scopes: "webhook.incoming"
};
```
