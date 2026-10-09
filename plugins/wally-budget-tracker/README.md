# Wally: Budget Tracker

Keep a personal budget in Wally: Budget Tracker from Claude Code. Tell Claude what you spent or
earned ("coffee 4.50 and taxi 12 yesterday"), ask how much went on food last month or what your
wallet balances are, and fix or delete a record by describing it. Records go into the same
encrypted backup in your Google Drive that the Wally app for Android and iOS syncs, so they show up
in the app after its next sync. The app is optional: your first record creates a wallet.

## Install

```
/plugin marketplace add aleksandrsvozn/watchmywallet-claude-plugin
/plugin install wally-budget-tracker@watchmywallet
```

## Sign in

Run `/mcp`, choose `wally` and sign in with Google. Use the account you sync the Wally app with, so
the chat and the app share the same records. Google asks for access to Wally's own folder in your
Drive; the connector can't see your other files.

## What the plugin contains

- One remote MCP server, `https://mcp.watch-my-wallet.com/mcp`, declared in `.mcp.json`.
- One skill with tips for Claude on how to use the server's tools.

The plugin runs no local code: no hooks, scripts or commands. Claude Code connects only to
`https://mcp.watch-my-wallet.com/mcp`, and only when Claude calls one of its tools.

## Bookkeeping only

Wally records expenses, income and transfers between your own wallets. It never moves money, makes
payments or connects to bank accounts.

## Examples

- "Coffee 4.50 and taxi 12 yesterday"
- "How much did I spend on food in September?"
- "I transferred 200 from my card to savings"
- "The taxi yesterday was 15, not 12"

## Privacy

The server reads and writes your encrypted backup only while it answers a request and does not
store your financial data. See Section 6B of the
[Privacy Policy](https://www.watch-my-wallet.com/privacy-policy.html#s6b) and
[how it works](https://www.watch-my-wallet.com/connect-ai.html).

Support: support@watch-my-wallet.com
