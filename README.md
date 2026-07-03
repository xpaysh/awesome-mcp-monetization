# Awesome MCP Monetization [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, protocols, platforms, and resources for monetizing [MCP](https://modelcontextprotocol.io/) (Model Context Protocol) servers.

MCP is rapidly becoming the standard for connecting AI agents to external tools. As the ecosystem grows, so does the need for sustainable business models around MCP servers. This list collects everything you need to monetize your MCP tools.

## Contents

- [Payment Protocols](#payment-protocols)
- [SDKs and Libraries](#sdks-and-libraries)
- [Platforms and Services](#platforms-and-services)
- [Server Registries](#server-registries)
- [Boilerplates and Templates](#boilerplates-and-templates)
- [Pricing Strategies](#pricing-strategies)
- [Tutorials and Guides](#tutorials-and-guides)
- [Community](#community)

## Payment Protocols

- [x402](https://github.com/coinbase/x402) - HTTP 402-based payment protocol by Coinbase. Enables native paywalls using USDC on Base. Designed for machine-to-machine payments.
- [Lightning/NWC](https://github.com/getAlby/awesome-nwc) - Nostr Wallet Connect enables Bitcoin Lightning micropayments for programmatic access. Sub-cent transaction costs.
- [Stripe Metered Billing](https://docs.stripe.com/billing/subscriptions/usage-based) - Traditional usage-based billing via API keys. Well-established infrastructure for fiat payments.

## SDKs and Libraries

- [MCPay](https://github.com/peterdev123/mcpay) - Payment gateway for MCP servers using the x402 protocol. Wraps existing servers with per-tool pricing.
- [PayMCP](https://github.com/paymcp/paymcp) - Provider-agnostic payment middleware supporting x402, Stripe, and wallet-based payments. Available in TypeScript and Python.
- [PaidMCP](https://github.com/paidmcp/paidmcp) - Lightning Network payments for MCP servers via Nostr Wallet Connect (NWC). Enables Bitcoin micropayments per tool call.
- [x402-mcp](https://github.com/AbanteAI/x402-mcp) - Three-line integration for monetizing MCP servers using the Vercel AI SDK and x402.
- [Coinbase Payments MCP](https://github.com/coinbase/coinbase-payments-mcp) - Full MCP server for cryptocurrency payments with companion wallet functionality.

## Platforms and Services

- [xpay](https://xpay.sh) - No-code MCP monetization platform. Register your server, set per-tool prices, and get a proxy URL in under 2 minutes. Supports fiat and crypto payments.
- [Nevermined](https://nevermined.io/) - AI-native billing infrastructure supporting usage-based, outcome-based, and value-based pricing models for AI services.
- [Moesif](https://www.moesif.com/) - API analytics and monetization platform with usage-based billing capabilities adaptable to MCP server metering.

## Server Registries

Registries where you can list and discover MCP servers, with notes on monetization support.

- [Official MCP Registry](https://github.com/modelcontextprotocol/registry) - The official registry for MCP servers maintained by Anthropic. Currently focused on discovery.
- [Smithery](https://smithery.ai/) - Registry with 7,300+ MCP servers. Includes server hosting and a managed proxy layer.
- [mcp.so](https://mcp.so/) - Community directory with 17,700+ servers. Focused on discovery and documentation.
- [Glama](https://glama.ai/mcp/servers) - MCP server registry with hosted proxy capabilities and usage analytics.
- [Toll402](https://toll402.com) — MCP server registry that only contains monetized MCP servers

## Boilerplates and Templates

- [paid-mcp-starter](https://github.com/xpaysh/paid-mcp-starter) - Ready-to-use templates showing three monetization approaches: no-code via xpay, x402 protocol, and Stripe billing. Includes a sample MCP server.
- [x402 Example Servers](https://github.com/coinbase/x402/tree/main/examples) - Official x402 example implementations from Coinbase showing payment-gated HTTP endpoints.
- [MCPay Examples](https://github.com/peterdev123/mcpay/tree/main/examples) - Example configurations for MCPay payment gateway integration.

## Pricing Strategies

Common approaches to pricing MCP server tools:

| Strategy               | Description                                          | Best For                                          |
| ---------------------- | ---------------------------------------------------- | ------------------------------------------------- |
| **Per-call flat rate** | Fixed price per tool invocation (e.g., $0.01/call)   | Simple tools with consistent compute cost         |
| **Per-token metered**  | Price based on input/output token count              | LLM-wrapper tools, text processing                |
| **Tiered pricing**     | Different price tiers based on volume                | High-volume enterprise users                      |
| **Freemium**           | Free credits on signup, paid after threshold         | Growing user base, low-friction onboarding        |
| **Dynamic pricing**    | Price adjusts based on complexity or demand          | Variable-cost tools (API aggregators, search)     |

## Tutorials and Guides

- [Coinbase x402 MCP Server Tutorial](https://docs.cdp.coinbase.com/x402/docs/x402-mcp-server) - Official guide to building an MCP server with x402 payment gating.
- [Vercel x402-mcp Integration](https://vercel.com/blog/x402-mcp) - Blog post on adding payment gates to MCP servers with 3 lines of code.
- [PaidMCP Lightning Tutorial](https://github.com/paidmcp/paidmcp#getting-started) - Getting started with Bitcoin Lightning payments for MCP servers.
- [xpay Monetize in 2 Minutes](https://xpay.sh/monetize-mcp-server) - No-code guide to monetizing any existing MCP server.
- [Building a Paid MCP Server from Scratch](https://github.com/xpaysh/paid-mcp-starter/blob/main/docs/pricing-guide.md) - Comprehensive guide to pricing strategies and implementation patterns.

## Community

- [MCP Discord](https://discord.gg/modelcontextprotocol) - Official Model Context Protocol community.
- [r/mcp](https://www.reddit.com/r/mcp/) - Reddit community for MCP discussion.
- [x402 Discord](https://discord.gg/cdp) - Coinbase Developer Platform community with x402 channels.

## Contributing

Contributions welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.
