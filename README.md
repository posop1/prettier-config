# `@posop/prettier-config`

> My personal [Prettier](https://prettier.io) configurations.
## Install

```sh
npm install @posop/prettier-config -D
```

```sh
yarn add @posop/prettier-config -D
```

```sh
pnpm add @posop/prettier-config -D
```

## Usage

### Overwrite some properties from the shared configuration

```js
// .prettierrc.js
module.exports = {
  ...require('@posop/prettier-config'),
}
```

### Copy the ignore file to your project folder

If you want to extend the ignore file, run the following command in the root of your project folder:

```bash
# unix
cp node_modules/@posop/prettier-config/.prettierignore .prettierignore
# windows
copy node_modules/@posop/prettier-config/.prettierignore .prettierignore
```

It will copy the `.prettierignore` from `@posop/prettier-config` to your project root folder.

### Scripts

Some commonly used scripts in `package.json`.

```json
{
  "scripts": {
    "format": "prettier --write --ignore-unknown **",
  }
}
```

### Rules
Rules used
```json
  "tabWidth": 2,
  "printWidth": 100,
  "semi": false,
  "useTabs": false,
  "singleQuote": true,
  "bracketSpacing": true,
  "bracketSameLine": false,
  "singleAttributePerLine": true,
  "arrowParens": "always",
  "trailingComma": "none",
  "quoteProps": "as-needed",
  "endOfLine": "lf",
```

## Related

- [Prettier](https://github.com/prettier/prettier) - an opinionated code formatter.
- [Prettier - Sharing configurations](https://prettier.io/docs/en/configuration.html#sharing-configurations) - Document on sharing prettier configurations.
- [Prettier - Ignore Code](https://prettier.io/docs/en/ignore.html) - Use `.prettierignore` to ignore certain files and folders completely.