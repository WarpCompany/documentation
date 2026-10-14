<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./logo/logo-white.svg" />
    <img src="./logo/logo-black.svg" alt="Warp" height="56" />
  </picture>
</p>

<h1 align="center">Warp Docs</h1>

<p align="center">
  Source for the Warp developer documentation at <a href="https://developer.usewarp.net">developer.usewarp.net</a>.
</p>

<p align="center">
  <a href="https://developer.usewarp.net"><img src="https://img.shields.io/badge/docs-developer.usewarp.net-B429FF" alt="Docs" /></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue" alt="License: MIT" /></a>
</p>

---

Warp is privacy-preserving payment and cross-chain infrastructure for developers. This repository contains the guides, product overviews, and API reference for:

- **Pay With Warp** — accept crypto payments from any supported chain
- **Warp Bridge** — move assets across chains
- **ZK Proofs as a Service** and the **ZK Validator Network** _(coming soon)_

## Local development

The site is built with [Mintlify](https://mintlify.com). You need Node.js 19 or later.

```bash
npm i -g mint
mint dev
```

The preview runs at `http://localhost:3000`.

## Structure

| Path               | Contents                                   |
| ------------------ | ------------------------------------------ |
| `docs.json`        | Site configuration and navigation          |
| `index.mdx`        | Landing page                               |
| `quickstart.mdx`   | Getting started guide                      |
| `products.mdx`     | Product overview                           |
| `warp-pay/`        | Pay With Warp guides and examples          |
| `warp-bridge/`     | Warp Bridge guides and protocol design     |
| `zkproofs/`        | ZK Proofs as a Service                     |
| `zkvalidator/`     | ZK Validator Network                       |
| `openapi.json`     | OpenAPI spec that powers the API reference |
| `images/`, `logo/` | Static assets                              |

New pages must be added to the `navigation` section of `docs.json` to appear in the sidebar.

## Contributing

Fixes and improvements are welcome. See [CONTRIBUTING.md](./CONTRIBUTING.md).

To report a security issue, follow [SECURITY.md](./SECURITY.md) instead of opening an issue.

## License

[MIT](./LICENSE)
