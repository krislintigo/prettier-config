# @krislintigo/prettier-config

Shared [Prettier](https://prettier.io) configuration.

## Installation

```bash
npm install -D prettier @krislintigo/prettier-config
```

## Usage

In `package.json`:

```json
{
  "prettier": "@krislintigo/prettier-config"
}
```

To extend the config, create a `prettier.config.js` file:

```js
export default {
  ...((await import('@krislintigo/prettier-config')).default),
  semi: true,
}
```

## Config

```json
{
  "printWidth": 100,
  "semi": false,
  "singleQuote": true,
  "trailingComma": "all",
  "htmlWhitespaceSensitivity": "ignore"
}
```
