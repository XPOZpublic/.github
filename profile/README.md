# Xpoz: social media data for AI agents

Xpoz gives AI agents and developers access to Twitter/X, Instagram, Reddit, and TikTok data: keyword search, user profiles, comments, engagement, and continuous tracking across billions of indexed posts. It works through a remote MCP server, a REST API, TypeScript and Python SDKs, and a CLI. No platform API keys, no scraping infrastructure to run.

## Connect in one minute

The MCP server is remote. Nothing to install; authentication is OAuth with a Google account on first connection.

**Claude Code**

```bash
claude mcp add --transport http --scope user xpoz https://mcp.xpoz.ai/mcp
```

**Claude Desktop**: Settings, Connectors, Add custom connector, URL `https://mcp.xpoz.ai/mcp`

**Cursor / VS Code / any MCP client**

```json
{ "mcpServers": { "xpoz": { "url": "https://mcp.xpoz.ai/mcp" } } }
```

**Python**

```bash
pip install xpoz
```

**TypeScript**

```bash
npm install @xpoz/xpoz
```

**CLI**

```bash
pip install xpoz-cli
# or
brew install XPOZpublic/xpoz/xpoz-cli
```

Want to test before signing up? A [trial token](https://docs.xpoz.ai/trial) works for 5 days with no signup and no credit card.

## What people use Xpoz for

- **Social listening and brand monitoring**: track keywords, hashtags, and accounts across all four platforms; new matching posts are collected automatically.
- **A Twitter/X API alternative**: search tweets by keyword, pull an account's posts, followers, retweeters, and quote tweets without an X developer account.
- **Historical Reddit data**: search posts and comments by keyword across subreddits, a common replacement for workflows that used Pushshift.
- **TikTok data without the Research API**: search by keyword, hashtag, sound, or creator.
- **Instagram keyword search**: find posts and profiles by keyword, read comments and interactions.
- **Connecting Claude, ChatGPT, or Cursor to live social media data**: the MCP server exposes 48 tools an agent can call directly.
- **Influencer discovery, sentiment analysis, and lead generation**: query in natural language, or use the ready-made [agent skills](https://github.com/XPOZpublic/xpoz-agent-skills).
- **Academic and market research**: export any query as CSV, or paginate through full result sets.

## Repositories

| Repo | What it is |
| --- | --- |
| [xpoz-mcp](https://github.com/XPOZpublic/xpoz-mcp) | The MCP server: 48 tools across Twitter/X, Instagram, Reddit, and TikTok |
| [xpoz-ts-sdk](https://github.com/XPOZpublic/xpoz-ts-sdk) | TypeScript SDK, `@xpoz/xpoz` on npm |
| [xpoz-python-sdk](https://github.com/XPOZpublic/xpoz-python-sdk) | Python SDK, `xpoz` on PyPI |
| [xpoz-cli](https://github.com/XPOZpublic/xpoz-cli) | Command-line client, `xpoz-cli` on PyPI and Homebrew |
| [xpoz-agent-skills](https://github.com/XPOZpublic/xpoz-agent-skills) | Agent skills for sentiment, influencer discovery, export, and OSINT |
| [xpoz-cookbooks](https://github.com/XPOZpublic/xpoz-cookbooks) | Jupyter notebooks: Xpoz with Claude, Gemini, and more |
| [geo-seo-agent](https://github.com/XPOZpublic/geo-seo-agent) | Open agent-operated GEO program that measures brand visibility in AI answers |
| [lead-gen-agent](https://github.com/XPOZpublic/lead-gen-agent) | Open agent-operated lead-generation loop over social buying-intent posts |

Integrations also ship for [Vercel AI SDK](https://github.com/XPOZpublic/ai-sdk), [LangChain](https://github.com/XPOZpublic/langchain-xpoz), [LlamaIndex](https://github.com/XPOZpublic/llama-index-tools-xpoz), [CrewAI](https://github.com/XPOZpublic/crewai-xpoz), [Dify](https://github.com/XPOZpublic/xpoz-dify-plugin), [Zapier](https://github.com/XPOZpublic/xpoz-zapier), [Cursor](https://github.com/XPOZpublic/xpoz-cursor-plugin), and [Claude Code](https://github.com/XPOZpublic/xpoz-claude-code-plugin).

## Pricing

The Free tier includes 500 credits with no credit card. Pro is $20/month (7,500 credits), Max is $200/month (120,000 credits). Credits are charged per query, not per result: Reddit and Twitter/X queries cost 2 credits, TikTok 5, Instagram 12. Full details at [xpoz.ai/pricing](https://www.xpoz.ai/pricing/).

## Links

- Documentation: [docs.xpoz.ai](https://docs.xpoz.ai)
- Website: [xpoz.ai](https://xpoz.ai)
- MCP endpoint: `https://mcp.xpoz.ai/mcp`
- REST API: [docs.xpoz.ai](https://docs.xpoz.ai) (bearer-key auth at `api.xpoz.ai`)
