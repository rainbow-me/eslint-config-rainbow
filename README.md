# eslint-config-rainbow
[![npm version](https://img.shields.io/npm/v/eslint-config-rainbow.svg)](https://npmjs.org/package/eslint-config-rainbow)
[![tests](https://github.com/rainbow-me/eslint-config-rainbow/actions/workflows/cd.yml/badge.svg)](https://github.com/rainbow-me/eslint-config-rainbow/actions/workflows/cd.yml)

A shareable [ESLint](https://github.com/eslint/eslint) config for Rainbow
projects.

## Usage

Install this package and its peer dependencies:

```sh
yarn add eslint-config-rainbow eslint jest react -D
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

## Contributing

This repo utilizes GitHub Actions and
[semantic-release](https://github.com/semantic-release/semantic-release) to
automatically test and publish this package to npm. Versioning is based on the
commit messages, which must follow the [Conventional
Commits](https://www.conventionalcommits.org/) standard i.e. `feat: <msg>` for
minor releases, `fix: <msg>` for patch.

When creating a PR, ensure that your commits follow these patterns. Upon merging
into `main`, your PR will be rolled up into a single release and published to
npm. Your release and changelog notes will then appear on the [releases
page](https://github.com/rainbow-me/eslint-config-rainbow/releases).
