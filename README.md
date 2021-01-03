# discord-slash-commands-helloworld

## Run locally

1. Set environment variables in `.env.json`

```json
{
    "SlashCommandsCallbackFunction": {
        "DISCORD_TOKEN": "...",
        "APPLICATION_ID": "...",
        "APPLICATION_PUBLIC_KEY": "...",
        "COMMAND_GUILD_ID": "..."
    }
}
```

2. Start local API using aws-sam-cli

:info: Use ngrok or something to bypass request verification!

```
$ sam local start-api --env-vars ./.env.json
```

## Deploy to AWS

```
$ sam build
$ sam deploy --guided
```
