# Contributing to Awesome Crypto MCPs

First — thank you for taking the time to contribute! This list only stays useful because of community curation.

## How to add an MCP

1. **Fork** this repo and create a new branch (e.g. `feature/add-foo-mcp`).
2. **Pick the right section.** Browse the README and add your MCP to the most relevant category. If your MCP truly doesn't fit any existing section, propose a new one in the PR description.
3. **Use the existing table format.** Match the columns and tone of the section you're adding to. Keep names short and capabilities skimmable.
4. **One line per MCP**, alphabetical within a logical sub-grouping where possible.
5. Use the **status legend**:
   - 🟢 Live — production-ready and actively maintained
   - 🟡 Beta / Preview — usable but rough edges or limited coverage
   - ⭐ Featured — only for the top featured slot (curator-only)

## Quality bar

Your MCP should:

- Implement the [Model Context Protocol](https://modelcontextprotocol.io/) spec.
- Have a public GitHub repo or a hosted endpoint (e.g. `https://mcp.example.io`).
- Provide clear setup / install instructions.
- Be related to crypto, blockchain, DeFi, NFTs, Web3, or directly useful to AI agents working with on-chain data.
- Not be abandoned. If the last commit is >12 months old and there are open critical issues, we may decline.

## What we *don't* accept

- Pure marketing pages with no working MCP.
- MCPs that aren't crypto/Web3-related.
- Duplicate entries (please check the list first).
- Affiliate-link spam or low-quality forks.

## Submitting a PR

1. Commit your changes with a clear message:
   ```
   git commit -m "Add FooMCP under DEX & On-Chain Trading MCPs"
   ```
2. Push to your fork and open a PR against `main`.
3. In your PR description, include:
   - Project name and link
   - One-line description of what the MCP does
   - Why it belongs in the section you placed it in

## Updating an existing entry

Found an outdated link, broken status, or wrong description? Open a PR with the fix and a brief note in the description (e.g. "Marked X as inactive — repo archived 2026-04").

## Reporting issues

Use the [Issues](../../issues) tab to:

- Report broken / dead MCPs
- Suggest new categories
- Propose corrections

Thanks for helping make this list great!
