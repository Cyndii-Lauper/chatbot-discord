# Discord Bot with OpenAI Integration

This Discord bot integrates with OpenAI's GPT-4 model to provide conversational AI capabilities in your server.

## Features

- Responds to messages in specified channels or when mentioned
- Uses OpenAI's GPT-4 model for generating responses
- Maintains conversation context from previous messages
- Splits long responses into multiple messages to comply with Discord's character limit

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js installed on your system
- A Discord bot token
- An OpenAI API key

## Installation

1. Clone this repository or download the source code.
2. Navigate to the project directory and run:

```
npm install
```

3. Create a `.env` file in the root directory with the following content:

```
TOKEN=your_discord_bot_token
OPENAI_KEY=your_openai_api_key
```

Replace `your_discord_bot_token` and `your_openai_api_key` with your actual Discord bot token and OpenAI API key, respectively.

## Configuration

In the main script, you can configure the following variables:

- `IGNORE_PREFIX`: Messages starting with this prefix will be ignored by the bot (default: "!")
- `CHANNELS`: An array of channel IDs where the bot will respond without being mentioned

## Usage

To start the bot, run:

```
node your_script_name.js
```

Replace `your_script_name.js` with the actual name of your script file.

The bot will respond in the specified channels or when mentioned in any channel. It ignores messages from other bots and messages starting with the ignore prefix.
