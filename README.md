# Wally: Budget Tracker for Claude Code

Ask about your spending and add expenses, income and transfers to
[Wally: Budget Tracker](https://www.watch-my-wallet.com) from Claude Code. The plugin connects the
Wally MCP server (`https://mcp.watch-my-wallet.com/mcp`) and teaches Claude how to use it.

## Install

```
/plugin marketplace add aleksandrsvozn/watchmywallet-claude-plugin
/plugin install wally@watchmywallet
```

Then run `/mcp`, choose `wally` and sign in with Google: the account you use for sync in the Wally
app. Without the app, your first record creates a wallet; install the app later and sign in with the
same Google account to see it there.

## Examples

- "Coffee 4.50 and taxi 12 yesterday"
- "How much did I spend on food in September?"
- "I moved 200 from my card to savings"
- "The taxi yesterday was 15, not 12"

## Privacy

The server reads and writes the encrypted backup in your Google Drive only while it answers a
request and does not store your financial data. See the
[Privacy Policy](https://www.watch-my-wallet.com/privacy-policy.html#s6b) and
[how it works](https://www.watch-my-wallet.com/connect-ai.html).

Support: support@watch-my-wallet.com
