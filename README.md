# Prettier Config

[Prettier](https://prettier.io/) is a highly effective tool that specializes in handling code formatting styles. :sparkles:
We have bundled our configuration to make it easily shareable across multiple projects.

- [Prettier Config](#prettier-config)
  - [Getting started](#getting-started)
  - [Config](#config)
  - [License](#license)

## Getting started

Install Prettier and the related configuration as a `devDependencies`:

```sh
# NPM
npm add --save-dev prettier @detra-lab/prettier-config

# PNPM
pnpm add --save-dev prettier @detra-lab/prettier-config

# Yarn
yarn add --dev prettier @detra-lab/prettier-config
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
npx prettier --write .
```

## Config

Check the [`.prettierrc.json`](./.prettierrc.json) file if you want to inspect the configuration.

## License

[MIT License](./LICENSE)
