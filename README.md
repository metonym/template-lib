# template-lib

[![Build Status](https://travis-ci.com/metonym/template-lib.svg?branch=master)](https://travis-ci.com/metonym/template-lib)

> Base template for developing npm libraries.

## Overview

### Develop

This command builds the project in watch mode. The source (i.e. entry) is in `src`, which is outputted in the designated folder `lib`.

```bash
yarn develop
```

### Build

This command first removes the `lib` folder before building the project.

```bash
yarn build
```

### Test

This command runs tests located in the `src/tests` folder.

```bash
yarn test
```

## Linting, formatting and committing

To ensure that committed code follows conventions, this project uses `prettier`, `tslint` and git hooks (via `husky`) to automate the linting and formatting of code and commit messages.

## License

[MIT](LICENSE)
