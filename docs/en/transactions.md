# Transactions

AturMyDuit records three transaction types: income, expense, and transfer.
Every change updates the related wallet balance immediately.

## Record a transaction

1. Tap the **+** button in the middle of the navigation bar.
2. Choose **Income**, **Expense**, or **Transfer**.
3. Fill in the amount, wallet, category, date, and an optional note.
4. Review the preview, then save.

Amounts are always whole rupiah. AturMyDuit does not use decimals.

## Income and expense

- **Income** adds to the wallet balance. Examples: salary, bonus, freelance.
- **Expense** subtracts from the wallet balance. Examples: food, transport,
  electricity.
- Categories separate income and expense. You can add, reorder, and archive
  categories in Settings.
- The system category **Biaya Admin** is used by transfers and cannot be
  deleted.

## Transfers

A transfer moves money between wallets in one operation:

- Two principal rows share one group: out of the source wallet and into the
  destination wallet.
- An admin fee, if any, is recorded as a separate expense.
- All rows are written in one database transaction, so a transfer is never
  half-finished.

See [Wallets and balances](wallets.md) for the full rules.

## Browse and search transactions

The **Transactions** tab shows every money record:

- Search by transaction name, merchant, or category.
- Filter by wallet, category, and period (this week, this month, this year, or
  all time).
- Tap a transaction to see its detail.

## Edit, delete, and undo

- A transaction can be edited from its detail page. The wallet balance follows.
- Deleting a transaction restores the wallet balance.
- Deletion offers **Undo** before the data is gone.
- Deleted data stays as a soft delete until you purge it from Settings.

## Bill payments

A bill payment appears as an expense transaction. If the payment is cancelled,
the transaction is removed and the bill returns to unpaid.
