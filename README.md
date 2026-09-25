# Telegram bot on GitHub Actions

This workflow runs the bot for up to about 5 hours and starts it again on a schedule. GitHub Actions does not guarantee a true 24/7 process, so this is a best-effort free option.

## Setup

1. Create or use a GitHub repository.
2. Upload `perfect.py`, `requirements.txt`, and `.github/workflows/bot.yml`.
3. In **Settings → Secrets and variables → Actions**, create a repository secret named `TELEGRAM_BOT_TOKEN`.
4. Paste the current bot token into that secret; do not commit it to the repository.
5. Open **Actions → Telegram bot → Run workflow** once to start it immediately.

The configured admin IDs are preserved in `perfect.py`.
