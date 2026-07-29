# Finance Tracker

A personal finance tracker — expenses by category, fixed/recurring payments
and subscriptions, credit card usage, and a dashboard of your current
financial status. Single self-contained page (`index.html`), no build step,
no server, no dependencies. All data is stored locally in your browser
(`localStorage`) on whichever device you open it on — nothing is ever sent
anywhere.

Live at: https://abdallahfauze.github.io/finance-tracker/

There's no bank/SMS integration — mobile platforms don't give apps access to
read your bank's text messages, so transactions are entered manually with
category auto-suggestion based on merchant keywords (editable in Settings).

Back up your data regularly via Settings → Save Backup (JSON), since this
page has no account or cloud copy of its own.
