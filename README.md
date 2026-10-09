# Wally: Budget Tracker for Claude Code

Ask about your spending and record expenses, income and transfers between your own wallets in
[Wally: Budget Tracker](https://www.watch-my-wallet.com) from Claude Code. The plugin connects the
Wally MCP server (`https://mcp.watch-my-wallet.com/mcp`) and teaches Claude how to use it. Wally is
bookkeeping only: it never moves money, makes payments or connects to bank accounts.

## Install

```
/plugin marketplace add aleksandrsvozn/watchmywallet-claude-plugin
/plugin install wally-budget-tracker@watchmywallet
```

Then run `/mcp`, choose `wally` and sign in with Google: the account you use for sync in the Wally
app. Without the app, your first record creates a wallet; install the app later and sign in with the
same Google account to see it there.

## Examples

- "Coffee 4.50 and taxi 12 yesterday"
- "How much did I spend on food in September?"
- "I transferred 200 from my card to savings"
- "The taxi yesterday was 15, not 12"

The plugin itself (in `plugins/wally-budget-tracker`) is described in its own [README](plugins/wally-budget-tracker/README.md).

## Privacy

The server reads and writes the encrypted backup in your Google Drive only while it answers a
request and does not store your financial data. See the
[Privacy Policy](https://www.watch-my-wallet.com/privacy-policy.html#s6b) and
[how it works](https://www.watch-my-wallet.com/connect-ai.html).

Support: support@watch-my-wallet.com
