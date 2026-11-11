# Veyndo Commerce

Run a shop or connect a component to the storefront you already have. Veyndo
brings native checkout, merchant Studio, apps and agents onto one Rust commerce
foundation.

[Try a hosted shop](https://start.veyndo.ai/start) · [Run Veyndo locally](https://www.veyndo.ai/docs/first-tour.html) · [Handbook](https://www.veyndo.ai/docs/) · [Überblick auf Deutsch](https://www.veyndo.ai/docs/platform-overview.html)

[![A shopper reviews price and delivery beside the Product Guide in the hosted Lumen shop](https://raw.githubusercontent.com/veyndo/veyndo/1d824485a47d6c23eb46260c651f42c5d5df492f/docs/assets/apps/product-guide-cart-review-20261111.jpg)](https://www.veyndo.ai/docs/status.html#product-guide-actions-in-the-hosted-shop)

## Public repositories

| Repository | Start here to… |
| --- | --- |
| [Veyndo Commerce](https://github.com/veyndo/veyndo) | Run the storefront, merchant Studio and commerce API. |
| [SDK](https://github.com/veyndo/sdk) | Connect a JavaScript or TypeScript app over HTTP and MCP. |
| [Apps](https://github.com/veyndo/apps) | Run app logic with Wasm and use scoped records, settings and durable jobs. |
| [Marketplaces](https://github.com/veyndo/marketplaces) | Sync listings and bring Amazon, eBay and Kaufland orders into a commerce host. |

The [component map](https://www.veyndo.ai/docs/one-shop-components.html) covers Checkout,
Knowledge, Automation, Connectors, EDI, Migration, POS, Shipping, Reports,
Payments and Experience. It includes the interfaces and access requirements.

## Follow one workflow

- **Shopper.** The Product Guide shows app results inside the conversation. The shopper reviews native price and delivery before confirming a cart addition. [Try the Product Guide](https://www.veyndo.ai/docs/product-guide-mcp-app.html).
- **Merchant.** Studio can read a private app note, propose a product edit and apply it after approval in a sandbox. [See the hosted check](https://www.veyndo.ai/docs/status.html#product-guide-actions-in-the-hosted-shop).
- **Developer.** The Connected Shop example uses the SDK to read the catalog, open an interactive MCP App and complete a simulated purchase through independent Checkout. [Read and run the example](https://www.veyndo.ai/docs/checkout-component.html#external-reference-storefront).

Native checkout and the original Storyfront use the same stock and order ledger.
The Lumen pilot records the running versions of its eight services and the
checks performed on them. [Release inventory](https://www.veyndo.ai/docs/components.json) ·
[Current acceptance](https://www.veyndo.ai/docs/status.html) · [Source license](https://www.veyndo.ai/docs/licensing.html).
