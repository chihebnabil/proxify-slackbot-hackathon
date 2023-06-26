## Overview

This is a Slack app built with the [Bolt for JavaScript framework][2] that showcases
responding to events and interactive buttons.

## Running locally

### 0. Create a new Slack App

- Go to https://api.slack.com/apps
- Click **Create App**
- Choose a workspace
- Enter App Manifest using contents of `manifest.yaml`
- Click **Create**

Once the app is created click **Install to Workspace** 
Then scroll down in Basic Info and click **Generate Token and Scopes** with both scopes

### 1. Setup environment variables

```zsh
# Replace with your bot and app token
export SLACK_BOT_TOKEN=<your-bot-token> # from the OAuth section
export SLACK_APP_TOKEN=<your-app-level-token> # from the Basic Info App Token Section
export SLACK_SIGNING_SECRET=
export OPENAI_API_KEY=
```

Or you can rename `.env.example` to `.env` and fill in the values.

### 2. Setup your local project

```zsh
# Clone this project onto your machine
git clone https://github.com/chihebnabil/proxify-slackbot-hackathon

# Change into the project
cd proxify-slackbot-hackathon/

# Install the dependencies
npm install
```

### 3. Start servers
```zsh
npm run start
```