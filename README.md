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
  <a href="https://developer.usewarp.net"><img src="https://img.shields.io/badge/docs-developer.usewarp.net-9E1FAA" alt="Docs" /></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue" alt="License: MIT" /></a>
</p>

---

Warp builds crypto payment and zero-knowledge infrastructure for developers. This repository contains the guides, product overviews, and API reference for:

- **Pay with Warp** — hosted crypto checkout on EVM chains
- **ZK Proofs** _(beta)_ — build, deploy and verify Circom/Groth16 circuits
- **Warp Verify** _(beta)_ — zero-knowledge attestations
- **Warp Bridge** and the **ZK Validator Network** _(roadmap)_

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
| `warp-pay/`        | Pay with Warp guides, embedded checkout, webhooks, examples |
| `sdks/`            | SDK guides                                 |
| `zkproofs/`        | ZK Proofs                                  |
| `warp-verify/`     | Warp Verify                                |
| `warp-bridge/`     | Warp Bridge design (roadmap)               |
| `zkvalidator/`     | ZK Validator Network design (roadmap)      |
| `api-reference/`   | API reference introduction                 |
| `openapi.json`     | OpenAPI spec that powers the API reference |
| `images/`, `logo/` | Static assets                              |

New pages must be added to the `navigation` section of `docs.json` to appear in the sidebar.

## Contributing

Fixes and improvements are welcome. See [CONTRIBUTING.md](./CONTRIBUTING.md).

To report a security issue, follow [SECURITY.md](./SECURITY.md) instead of opening an issue.

## License

[MIT](./LICENSE)
