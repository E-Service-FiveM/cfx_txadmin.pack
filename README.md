Here’s the `README.md` file for your GitHub repository:

```markdown
# TxAdmin Logging Script by Novek

This script allows you to monitor events from `txAdmin` and send important actions such as player warnings, bans, and whitelist requests to a Discord webhook. It provides an easy way to monitor activities on your server and receive real-time notifications.

## Features

- **Event Logging**: Sends logs of player warnings, bans, whitelist requests, and announcements to Discord.
- **Custom Webhook Integration**: You can specify a Discord webhook to receive notifications.
- **Multi-language Support**: Currently, the script supports English and German. More languages can be added easily.
- **Simple Configuration**: All settings, including the webhook and logo, can be easily customized.

## Installation

1. **Download the files**:
   Download the script and its files, and place them in the `resources/` folder of your server.

2. **Activate the resource**:
   Make sure to add the resource in your `server.cfg` with the following command:

   ```plaintext
   ensure txadmin logging
   ```

3. **Insert the Webhook URL**:  
   Open the file `resources/txadmin/shared/config.lua` and enter your Discord webhook URL:  
   ```lua
   Noveks_CFG.txAdminWebhook = 'YOUR_WEBHOOK_URL'
   ```

4. **Customize the Logo URL**:  
   If you want to use a custom logo for the Discord messages, you can also edit the `Logo` URL in the config file:  
   ```lua
   Noveks_CFG.Logo = 'YOUR_LOGO_URL'
   ```

## Configuration

The configuration file is located at `resources/txadmin/shared/config.lua`. Here you can adjust the following parameters:

- **txAdminWebhook**: Your Discord webhook URL.
- **Username**: The username that will be shown in Discord messages.
- **Logo**: The URL to your server logo that will be shown in Discord messages.
- **FilterAnnouncements**: Whether announcements are only shown by admins (`true/false`).
- **Locale**: Set the language for the messages (e.g., `'en'` for English, `'de'` for German).

## Events

The script monitors and logs the following events:

- **Player warnings**: Sends notifications when a player is warned.
- **Player bans**: Sends notifications when a player is banned.
- **Whitelist Requests**: Logs and sends notifications for whitelist requests.
- **Announcements**: Monitors server announcements and sends notifications.
- **Configuration Changes**: Sends notifications when changes are made.
- **Player Healing**: Notifies when a player is healed.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
```

This `README.md` contains all necessary information and formatting for users to install and configure the script on their server.
