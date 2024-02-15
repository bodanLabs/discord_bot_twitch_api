# Discord Twitch Notification Bot

This Discord bot is designed to monitor Twitch streamers and notify a Discord channel when specified streamers go live. It uses the Twitch API to check the live status of streamers and Discord's API to send notifications to a guild (server).

## Features

- Twitch streamer live status monitoring.
- Automatic notifications in Discord channels when streamers go live.
- Ability to add Twitch streamer names to the monitoring list via a Discord command.

## Requirements

- Python 3.6 or newer
- discord.py
- twitchAPI
- requests

## Setup Instructions

1. **Clone the Repository:**

    ```
    git clone <repository-url>
    ```

2. **Install Dependencies:**

    Ensure you have Python 3.6 or newer installed. Then, run:

    ```
    pip install discord.py twitchAPI requests
    ```

3. **Twitch API Credentials:**

    You will need to create a Twitch application at [Twitch Developers](https://dev.twitch.tv/console/apps) to get your client ID and client secret.

4. **Discord Bot Token:**

    Follow the instructions at [Discord's Developer Portal](https://discord.com/developers/applications) to create a bot and get your token.

5. **Configuration:**

    Replace the placeholders in the script with your actual Twitch client ID, client secret, and Discord bot token.

    - `TOKEN` with your Discord bot token.
    - `client_id` and `client_secret` with your Twitch application credentials.

6. **Running the Bot:**

    Run the bot with the following command:

    ```
    python bot.py
    ```

## Usage

- **Add Twitch Streamer to Notifications:**

    Use the `$addtwitch <TwitchUsername>` command in your Discord server to add a Twitch streamer to the notification list.

- **Live Notifications:**

    The bot will automatically check for streamers' live status every 10 seconds and notify the designated Discord channel when a streamer goes live.

## Contribution

Contributions are welcome! If you have suggestions for improvements or bug fixes, please open an issue or submit a pull request.

## Disclaimer

This project is not affiliated with Discord or Twitch. It is a community-driven project intended for educational purposes.

