# tacobot

This repository is simply a `docker-compose` configuration file to create and
run containers for:

1. [tacoday-api](https://github.com/misterdjules/tacoday-api), a simplistic API
server that uses Facebook's API to get special deals from La Taqueria, a tacos
restaurant in Vancouver.

2. [taco-slackbot](https://github.com/misterdjules/taco-slackbot), a Slack bot
that uses this API server and gives information about the special deals of the
day to users in a Slack chat room.

It is a toy project used to experiment with using containers to deploy
software.

## Creating and running all containers

```
SLACK_TOKEN=your_slack_tocken FB_APP_TARGET_PAGE=LaTaqueria FB_APP_TOKEN=your_fb_app_access_token docker-compose up -d taco-slackbot
```
