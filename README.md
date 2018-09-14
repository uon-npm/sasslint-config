[![NPM](https://nodeico.herokuapp.com/@universityofnottingham/sasslint-config.svg)](https://npmjs.com/package/@universityofnottingham/sasslint-config)

## University of Nottingham standard `sass-lint` configuration

> to prevent the same `.sass-lint.yml` being present on every project with any SCSS in.

## Usage

In an `npm` enabled project:

1. Have `sass-lint`
    - `npm i -D sass-lint`
1. Install this package
    - `npm i @universityofnottingham/sasslint-config`
1. Add `sasslintConfig` to `package.json` referring to the config in this package:

```js
{
  //...
  "sasslintConfig": "./node_modules/@universityofnottingham/sasslint-config/.sass-lint.yml"
  //...
}
```

Enjoy your lightweight, UoN standard `sass-lint` without a separate config file!

## Optional overrides / extensions

1. Create a new local `.sass-lint.yml` for your project
1. Remove `sasslintConfig` from `package.json`
1. Refer to the config in this package from your local `.sass-lint.yml`:

```yaml
options:
  config-file: "./node_modules/@universityofnottingham/sasslint-config/.sass-lint.yml"
  #...
rules:
  # optional rule overrides
```