# XaviaBot - Web Chat Mode

Your personal bot running on Replit with a built-in web chat UI.
**No Facebook login required!**

## Setup on Replit

1. Upload this folder to Replit
2. In Replit Shell, run:
   ```
   npm install
   ```
3. Click **Run** (or run `npm start`)
4. Open the Replit web preview — your chat UI will appear

## How it works

- The bot runs on Replit as a Node.js server
- You open the web URL Replit gives you
- You chat directly in the browser — the bot reads your messages and replies in real time
- All your existing commands/plugins still work the same way!

## Using Commands

Use the prefix defined in `config/config.main.json` (default: `x`)

Example: `xhelp`, `xping`, etc.

## Customizing

- Change bot name: Edit `"NAME"` in `config/config.main.json`
- Change prefix: Edit `"PREFIX"` in `config/config.main.json`
- Change timezone: Edit `"timezone"` in `config/config.main.json`
- Add plugins: Drop them in `plugins/commands/`

## Notes

- The old Facebook appstate/cookie login has been completely removed
- The `@xaviabot/fca-unofficial` package is no longer needed
- Socket.io handles all real-time messaging between your browser and the bot
