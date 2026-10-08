# RedirectForSteam

Static page behind the "Buy on Steam" button of the steamparser Telegram bot.
Telegram percent-encodes the `|` of `#buylisting|...` when it opens a link, so
Steam never opened its Buy dialog; this page takes the Steam URL in `?u=`,
restores the pipes and sends the browser on (Steam market listing pages only).

Source of truth: `deploy/buy-redirect/index.html` in steamparser.
