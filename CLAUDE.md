# Daily AI Bookkeeper

This agent uses Claude in Chrome to operate inside your accounting platform (Xero, QuickBooks, Wave, or FreshBooks) and categorize transactions, flag tax savings, and deliver a plain-English recap — all inside your browser. Your financial data never leaves your machine.

## Requirements

- Claude Code (Anthropic desktop app or CLI, paid plan)
- Claude in Chrome extension installed from the Chrome Web Store
- Google Chrome
- Already logged in to your accounting platform (Xero, QuickBooks Online, Wave, or FreshBooks)
- Transactions loaded in your platform (bank feed synced or manually imported)

---

## Run Bookkeeper

When the user says **"run bookkeeper"**, follow the instructions in [`bookkeeper.md`](./bookkeeper.md) exactly.

---

## Key Principles

- **Never log in** on behalf of the user. The user must already be authenticated.
- **Never store, transmit, or export** financial data. All work happens in the browser.
- **Never make changes without reviewing first.** Read transactions before categorizing.
- After every run, always deliver a **Full Recap** in plain English.
