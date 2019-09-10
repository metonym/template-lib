# template-lib

[![Build][build]][build-badge]
[![Coverage][codecov-shield]][codecov]

> Template for developing libraries in TypeScript and publishing on [npm](https://www.npmjs.com/).

## Available Scripts

### `yarn develop`

Runs the project in development mode. TypeScript watches `src/` and rebuilds on changes.

### `yarn build`

Builds the project for production using `tsconfig.prod.json`. The extended configuration ignores `src/tests`.

```json
// tsconfig.prod.json
{
  "extends": ".",
  "exclude": ["src/tests"]
}
```

### `yarn lint`

Runs [TSLint](https://github.com/palantir/tslint) on `src/` and fixes errors (if fixable).

### `yarn test`

Runs test using [Jest](https://jestjs.io/).

## Linting, formatting and committing

To ensure that committed code follows conventions, this project uses `prettier`, `tslint` and git hooks (via `husky`) to automate the linting and formatting of code and commit messages.

## License

[MIT](LICENSE)

[build]: https://travis-ci.com/metonym/template-lib.svg?branch=master
[build-badge]: https://travis-ci.com/metonym/template-lib
[codecov]: https://codecov.io/gh/metonym/template-lib
[codecov-shield]: https://img.shields.io/codecov/c/github/metonym/template-lib.svg
