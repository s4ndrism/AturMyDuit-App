# Budgets and bills

The **Budget** tab holds two things: spending limits and recurring bills.

## Budgets

A budget is a spending limit, not an allocation of income.

1. Open the **Budget** tab.
2. Tap **Add budget**.
3. Fill in the name, spending limit, and start date.
4. Choose the scope: all categories (overall) or a specific category.
5. Optionally limit it to one wallet.
6. Save.

Good to know:

- A per-category budget is more specific than an overall budget.
- Actual spending is calculated from expenses in the current period.
- Transfer principal is not counted as an expense. The admin fee still is.
- A budget can be deactivated without being deleted. Inactive budgets are not
  shown in the summary.
- Deleting a budget does not delete old transactions.

## Bills

Bills are for recurring expenses such as internet, electricity, rent, or
subscriptions.

1. Open the **Bills** tab inside Budget.
2. Tap **Add bill**.
3. Fill in the name, amount, first due date, and time.
4. Pick the expense category and payment wallet.
5. Set the recurrence: daily, weekly, monthly, or yearly.
6. Turn on **Auto pay** if the bill should be recorded automatically when due.
7. Save.

### Schedule and due dates

- The schedule is calculated from the start date, not from the last due date.
- The end date is optional. Without it, the bill keeps running.
- A paused bill creates no new schedule and is not auto-paid.
- Changing the amount does not change bills that already passed.

### Pay, skip, and cancel

- **Pay manually** creates an expense transaction and marks the bill paid.
- **Skip** skips one due date without creating a transaction.
- Cancelling a payment removes the transaction and returns the bill to unpaid.
- If the balance is not enough during auto pay, the bill is marked failed
  without creating a transaction.

### H-24 reminder

AturMyDuit sends a reminder one day before the due date. Allow notifications
for AturMyDuit in Android settings. If notifications only appear in the panel
and not as a pop-up, enable **Pop on screen** for AturMyDuit.

In debug mode, Settings has a **Test bill notification** button to confirm that
the permission and notification channel work.
