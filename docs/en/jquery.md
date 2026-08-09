# @ares/jquery Documentation

## Purpose

JQuery for cheerio parsing

## Installation

```bash
yarn add @ares/jquery
```

In a Yarn Workspaces monorepo:

```bash
yarn workspace <app> add @ares/jquery
```

## Quickstart

Minimal example:

```js
import * as mod from "@ares/jquery";
```

## Public API (exports)

This section documents the actual public surface at entrypoint level and main exported symbols.

Root entrypoint:

- `@ares/jquery`

Main files at package root (indicative):

- `index.js`

Exports detected in `index.*`:

- `parse`
- `parseCode`
- `parseFile`
- `parseUrl`

## Configuration (appSetup / config / policies)

This module may read configuration from `appSetup`, `config`, or `policies` depending on the type. Document the actually consumed keys as you stabilize the contract.

## Test

Run module tests (if present):

```bash
yarn workspace @ares/jquery test
```

## Notes

- This document is maintained alongside the module tickets.
