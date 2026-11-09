# Veyndo Commerce

Veyndo is an AI-native commerce platform you can run as one shop or use in parts. Build a storefront, run the merchant workspace, and let agents work with the same catalogue, rules and approved operations your team uses.

[Try Veyndo](https://start.veyndo.ai/) · [Read the handbook](https://www.veyndo.ai/docs/) · [Check the current status](https://www.veyndo.ai/docs/status.html)

## Find your starting point

| Repository | Start here if you want to… |
| --- | --- |
| [veyndo](https://github.com/veyndo/veyndo) | Run the complete shop, merchant Studio and commerce API. |
| [sdk](https://github.com/veyndo/sdk) | Call Veyndo and independently hosted components from JavaScript or TypeScript over HTTP and MCP. |
| [apps](https://github.com/veyndo/apps) | Run app logic in a bounded Wasm runtime or use the shared storage for records, settings and jobs. |
| [marketplaces](https://github.com/veyndo/marketplaces) | Map products, sync listings and bring marketplace orders into a commerce host. |

The [component map](https://www.veyndo.ai/docs/one-shop-components.html) also covers Checkout, Knowledge, Automation, Connectors, EDI, Migration, POS, Shipping, Reports, Payments and Experience. It distinguishes public repositories, access-controlled services and planned boundaries.

If you already have a storefront, follow the [Checkout browser example](https://www.veyndo.ai/docs/checkout-component.html#external-reference-storefront). It shows where the JavaScript SDK connects to Checkout and how the commerce host supplies the price, confirms the purchase and returns the original receipt.

If you are building an assistant, the [Knowledge component guide](https://www.veyndo.ai/docs/knowledge-component.html) shows how to search private sources with the SDK and verify a passage against its current revision.

The [Automation component guide](https://www.veyndo.ai/docs/automation-component.html) shows how to preview a rule from an external application and how that same evaluator fits into checkout and Flows.
If you're building a Flow editor, read trigger and action names from the [built-in Flow catalog](https://www.veyndo.ai/docs/automation-component.html#built-in-flow-catalog). Then [check the draft through Core](https://www.veyndo.ai/docs/automation-component.html#check-a-flow-draft-before-saving) before saving. Your editor and Studio use the same rules and current shop permissions.

If you're connecting email, Slack or other providers, start with the [Connector guide](https://www.veyndo.ai/docs/connector-component.html). It explains how to keep an existing Veyndo installation on its current queue, or run the Connector with its own database and scoped HTTP and MCP access.

## How the pieces fit

A storefront, a register and an assistant can use the same shop. Commerce owns authoritative prices, inventory and orders. Checkout orchestrates the buyer journey. After the order commits, a background worker picks up its Flow and saves progress in PostgreSQL. You can run that worker separately from the storefront API. It continues from the saved step after a restart. The handoff guide shows how to move app work out of Core while checkout keeps accepting orders. [Worker handoff](https://www.veyndo.ai/docs/automation-component.html#move-the-app-worker-out-of-core). Apps and provider adapters can act on those events, and agents prepare changes within their grants. [Flow worker and Rust contract](https://www.veyndo.ai/docs/automation-component.html#portable-flow-directives).

Start with the [architecture](https://www.veyndo.ai/docs/architecture.html) for the ownership boundaries, the [quick start](https://www.veyndo.ai/docs/quickstart.html) for a local shop, and the [issue tracker](https://github.com/veyndo/veyndo/issues) to discuss a reproducible problem or proposed change.
