# Getting started

## Install the app

1. Open the [releases page](https://github.com/s4ndrism/AturMyDuit-App/releases/latest).
2. Download `AturMyDuit-1.0.0.apk` and `SHA256SUMS.txt`.
3. Allow installs from unknown sources in your Android settings.
4. Open the APK and finish the installation.
5. Optionally verify the checksum against `SHA256SUMS.txt`:

   ```powershell
   Get-FileHash AturMyDuit-1.0.0.apk -Algorithm SHA256
   ```

AturMyDuit is Android only. The APK is signed with the release keystore, so
future updates can be installed over the previous version.

## First launch

On first launch, AturMyDuit creates one wallet named **Cash** with a zero
balance. You can use it right away or add another wallet.

Suggested order:

1. Open **Wallets** and set the opening balance for the wallet you use.
2. Record your first income or expense with the **+** button.
3. Set a monthly budget in the **Budget** tab.
4. Add recurring bills if you have any.
5. Set your profile, theme, and language in **Settings**.

## Main screens

- **Home**: greeting, Total Duit, transaction summary, budget, and bills.
- **Charts**: income and expense reports.
- **Budget**: budgets and the bill list.
- **Transactions**: the full transaction history.
- **+ button** in the middle of the navigation bar: record income, expense,
  or a transfer.
- **Profile icon** on Home: opens Settings.

## Opening balance

The opening balance is not a separate column. When you set the first balance,
AturMyDuit creates an adjustment row named "Saldo awal". Later balance
corrections also create new adjustment rows, so old history is never edited.
