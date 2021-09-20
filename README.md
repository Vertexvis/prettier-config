# @vertexvis/prettier-config

Vertex's shared Prettier config.

## Usage

This is based on [Shared
Configurations](https://prettier.io/docs/en/configuration.html#sharing-configurations)
in Prettier's documentation.

1. Remove any existing `.prettierrc` files.
2. Install the config.
  ```
  yarn add --dev @vertexvis/prettier-config

  # or

  npm install -D @vertexvis/prettier-config
  ```
3. Update your `package.json` to reference the shared config.
  ```
  "prettier": "@vertexvis/prettier-config",
  ```

## Overrides

If you'd like to override any of the default settings, add a `.prettierrc.js`
file in your project with any settings that you'd like to change:

```js
module.exports = {
  ...require("@vertexvis/prettier-config"),
  semi: false,
};
```

## Publishing to NPM

To publish a release to NPM, run `yarn version` to update the major or minor
version. Commit your changes and open a PR. Once the PR is merged, the new
version will be published to NPM.
