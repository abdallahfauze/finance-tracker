# Finance Tracker

A finance tracker — expenses by category, fixed/recurring payments and
subscriptions, credit card usage, budgets, and a dashboard of your current
financial status. Single self-contained page (`index.html`), no build step,
no server framework, no dependencies beyond Firebase.

Live at: https://abdallahfauze.github.io/finance-tracker/

Each person signs up with their own email + PIN (a real Firebase Auth
account under the hood, so the PIN is genuinely verified server-side). Data
syncs in real time via Firestore, scoped per-account by security rules so
nobody can read or write anyone else's data, and is also cached in
`localStorage` for instant loads and offline use.

There's no bank/SMS integration — mobile platforms don't give apps access to
read your bank's text messages, so transactions are entered manually with
category auto-suggestion based on merchant keywords (editable in Settings).

Back up your data regularly via Settings → Save Backup (JSON) as a second
copy, since it's still worth having outside the cloud sync.
