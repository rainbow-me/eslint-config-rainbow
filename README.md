# eslint-config-rainbow

A shareable [eslint](ghub.io/eslint) config for Rainbow projects.

## Usage

Install into your project:

```sh
yarn add --dev prettier eslint eslint-config-rainbow
```

Then extend your `.eslintrc.js` config:

```js
module.exports = {
  extends: "rainbow"
}
```

Add a step to your `package.json` to lint your project:

```json
{
  "scripts": {
    "lint": "eslint --ext '.ts,.tsx,.js,.jsx' ."
  }
}
```

## See also

`eslint-config-rainbow` is based on [`eslint-config-satya164`](https://ghub.io/eslint-config-satya164) but with flow removed and slightly modified to work better for rainbow projects.
