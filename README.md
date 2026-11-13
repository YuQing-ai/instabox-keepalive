# instabox-keepalive

This repository only keeps the InstaBox machine awake via its official wake API, using GitHub Actions every 10 minutes.

No secrets are stored in code. The API key is stored as the GitHub Actions secret `INSTABOX_API_KEY`, and the machine ID is stored as the variable `INSTABOX_MACHINE_ID`.

The workflow pauses once every 6 hours (off-windows 08:00-08:40, 14:00-14:40, 20:00-20:40, 02:00-02:40 CST).
