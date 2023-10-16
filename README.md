# Prettier Config

[![NPM Version][npm_version_badge]][npm_badge_url]
[![NPM Downloads][npm_downloads_badge]][npm_badge_url]

[Prettier](https://prettier.io/) is a highly effective tool that specializes in handling code formatting styles. :sparkles:
We have bundled our configuration to make it easily shareable across multiple projects.

- [Prettier Config](#prettier-config)
  - [Getting started](#getting-started)
  - [Config](#config)
  - [Code of Conduct](#code-of-conduct)
  - [License](#license)

## Getting started

Install Prettier and the related configuration as a `devDependencies`:

```sh
pnpm add -D @detra-lab/prettier-config prettier
```

Reference it in your `package.json`:

```json
{
  "name": "my-cool-library",
  "version": "1.0.0",
  "prettier": "@detra-lab/prettier-config"
}
```

If you don’t want to use `package.json`, you can choose any of the [supported extensions](https://prettier.io/docs/en/configuration) to export a string, e.g. `.prettierrc.json`:

```json
"@detra-lab/prettier-config"
```

> Note: This method doesn't offer a way to extend the configuration and override some properties. If you need to do that, import the file in a `.prettierrc.js` file and export the modifications:

```js
module.exports = {
  ...require('@detra-lab/prettier-config'),
  semi: true
};
```

Use the `--write` flag to format a file in place.

```sh
pnpx prettier . --write --ignore-unknown
```

## Config

Check the [`.prettierrc.json`](https://github.com/detra-lab/prettier-config/blob/stable/.prettierrc.json) file if you want to inspect the configuration.

## Code of Conduct

Help us keep the project open and inclusive. Please read and follow our [Code of Conduct](https://github.com/detra-lab/prettier-config/blob/stable/CODE_OF_CONDUCT.md).

## License

[Apache License 2.0](https://github.com/detra-lab/prettier-config/blob/stable/LICENSE)

<div align="center"><img src="https://raw.github.com/detra-lab/.github/stable/profile/logo.svg" width="100" height="100" alt="Detra" /><p><small>© 2023 Detra</small></p></div>

<!-- Badges -->
[npm_version_badge]: https://img.shields.io/npm/v/@detra-lab/prettier-config?style=flat-square&colorA=424394&colorB=80ffdb
[npm_downloads_badge]: https://img.shields.io/npm/dm/@detra-lab/prettier-config?style=flat-square&colorA=424394&colorB=80ffdb

<!-- Links -->
[npm_badge_url]: https://www.npmjs.com/package/@detra-lab/prettier-config
