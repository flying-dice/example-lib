# @flying-dice/example-lib

An example library repo demonstrating how to publish a TypeScript package as a GitHub dependency using Bun and semantic-release.

## Features

- Installable directly from GitHub (no npm publish required)
- Automated versioning and tagging via [semantic-release](https://github.com/semantic-release/semantic-release)
- Uses [conventional commits](https://www.conventionalcommits.org/) to determine version bumps

## Installation

Latest version:

```bash
bun add github:flying-dice/example-lib
```

Pinned to a specific version tag:

```bash
bun add github:flying-dice/example-lib#v1.0.0
```

## Usage

```ts
import { greet } from "@flying-dice/example-lib";

console.log(greet("world")); // Hello, world!
```

## Versioning

This repo uses semantic-release with conventional commits:

- `fix: ...` — patch release (e.g. `1.0.0` -> `1.0.1`)
- `feat: ...` — minor release (e.g. `1.0.0` -> `1.1.0`)
- `feat!: ...` or `BREAKING CHANGE:` — major release (e.g. `1.0.0` -> `2.0.0`)