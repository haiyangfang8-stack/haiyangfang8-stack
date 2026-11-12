# 每天八点起床 · EightAM

**把没有 API 的中国数据源，接给 AI。**

China publishes an enormous amount of public data — tenders, policies, registries — behind
systems that have no API, no docs and no export. I build adapters that expose them to AI
agents through [MCP](https://modelcontextprotocol.io), so an LLM can query real, live data
instead of guessing.

## Projects

| Project | Data source | What an AI can do with it |
|---|---|---|
| [**ggzy-mcp**](https://github.com/haiyangfang8-stack/ggzy-mcp) | 全国公共资源交易平台 | 查任意关键词/省份/时间段的招标公告，带原始链接 |
| [**gov-policy-mcp**](https://github.com/haiyangfang8-stack/gov-policy-mcp) | 中国政府网政策文件库 | 检索国务院文件，返回文号、发文机关、成文日期 |

Both are MIT, run locally over stdio, and need no API key.

## How they are built

1. **Find the XHR** the site's own frontend already calls — no scraping rendered HTML
2. **Replay it server-side** with the right headers; no browser, no login
3. **Map the fields**, strip HTML noise, normalise dates and relative URLs
4. **Wrap in an MCP tool** with a schema an LLM can reason about
5. **Format the output for reading**, not for parsing — an LLM should not need to decode JSON

The pattern is identical every time, which is why a new adapter takes about a day.

## Skills

`TypeScript` · `Node.js` · `Python` · `MCP` · `web reverse engineering` ·
`Android (jadx / apktool / Frida)` · `data pipelines`

## Work with me

If you have a system with data you need in an AI workflow but no API to reach it,
that is exactly the problem I solve.

- WeChat: `2450175024`
- Email: `2450175024@qq.com`
