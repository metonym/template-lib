# template-lib

[![Build][build]][build-badge]
[![Coverage][codecov-shield]][codecov]

> Template for developing libraries in TypeScript and publishing to [npm](https://www.npmjs.com/).

## Available Scripts

### `yarn build`

Builds the project for production.

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

Runs the `prepublishOnly` command, which first builds the project for production before publishing the library.

## Linting, formatting and committing

To ensure that committed code follows conventions, this project uses `prettier`, `tslint` and git hooks (via `husky`) to automate the linting and formatting of code and commit messages.

## License

[MIT](LICENSE)

[build]: https://travis-ci.com/metonym/template-lib.svg?branch=master
[build-badge]: https://travis-ci.com/metonym/template-lib
[codecov]: https://codecov.io/gh/metonym/template-lib
[codecov-shield]: https://img.shields.io/codecov/c/github/metonym/template-lib.svg
