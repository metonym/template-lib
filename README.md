# template-lib

[![Build][build]][build-badge]

> Template for developing libraries in TypeScript and publishing to [npm](https://www.npmjs.com/).

## Getting Started

Scaffold a new project using npx and degit:

```bash
npx degit metonym/template-lib template-lib
cd template-lib
yarn
```

## Available Scripts

### `yarn test`

Runs test using [Jest](https://jestjs.io/) and generates a code coverage report.

### `yarn test:tdd`

Runs tests in "Test-driven Development Mode."

## Publishing to NPM

You must create an NPM account before publishing packages on the NPM registry.

In [package.json](package.json), customize the following metadata before publishing to NPM.

```json
{
  "repository": {
    "type": "git",
    "url": "https://github.com/{USER-NAME}/{REPO-NAME}.git"
  },
  "homepage": "https://github.com/{USER-NAME}/{REPO-NAME}",
  "keywords": ["..."],
  "bugs": "https://github.com/{USER-NAME}/{REPO-NAME}/issues"
}
```

### `yarn publish`

Runs the `prepack` command, which first builds the project for production before publishing the library.

## License

[MIT](LICENSE)

[build]: https://travis-ci.com/metonym/template-lib.svg?branch=master
[build-badge]: https://travis-ci.com/metonym/template-lib
