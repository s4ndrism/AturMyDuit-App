# FAQ

## Is my data uploaded to a server?

No. Every transaction, wallet, budget, bill, and profile stays in a local
database on your phone. There is no account and no server sync.

The only network access is the update check. The app reads public release
metadata from `api.github.com`. No transactions, identity, or analytics are
sent.

## Can the app work offline?

Yes. All core features work without internet. Only the update check needs a
connection, and its failure never blocks the app.

## Why does a wallet balance not match?

Balances come from the ledger. Check:

1. income and expense transactions in that wallet;
2. incoming and outgoing transfers, including admin fees;
3. the "Saldo awal" adjustment and any balance corrections.

If needed, create a new correction from the transaction screen. Do not edit old
history.

## Is a transfer counted as an expense?

No. Transfer principal only moves money between wallets. The admin fee is the
only part counted as an expense.

## What if the balance is not enough?

A wallet rejects transactions that would make the balance negative, unless
**Allow negative balance** is enabled.

## How do I keep my data safe?

Create a local backup regularly from **Settings > Backup & Restore**, then keep
a copy somewhere else. Backups are not encrypted yet.

## Is the APK on the Play Store?

For 1.0.0, the APK is distributed through GitHub Releases. Download it from the
public `AturMyDuit-App` repository, verify the checksum, and install it
manually.

## Why is there an unknown source warning?

Android shows that warning for APKs installed outside the Play Store. Allow
installs from unknown sources only for apps you trust.

## Is the app free?

AturMyDuit is free for personal and non-commercial use. The source code is
proprietary. Donations through Trakteer are optional.

## How do I report a bug?

Open an [issue](https://github.com/s4ndrism/AturMyDuit-App/issues). Include the
app version, phone model, Android version, and steps to reproduce the problem.
Never attach personal transactions or backup files.
