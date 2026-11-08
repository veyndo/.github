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

## How the pieces fit

A storefront, a register and an assistant can use the same shop. Commerce owns authoritative prices, inventory and orders. Checkout orchestrates the buyer journey. Apps and background workers extend what the shop can do. Agents can read within their grants and prepare changes for review. The checkout and merchant operations apply the same rules regardless of which interface initiated them.

Start with the [architecture](https://www.veyndo.ai/docs/architecture.html) for the ownership boundaries, the [quick start](https://www.veyndo.ai/docs/quickstart.html) for a local shop, and the [issue tracker](https://github.com/veyndo/veyndo/issues) to discuss a reproducible problem or proposed change.
