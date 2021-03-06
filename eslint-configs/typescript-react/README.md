# @kwizapp/eslint-config-ts-react

[Link to Package](https://github.com/kwizapp/kwiz-dotfiles/packages/160123)

### Typescript React

This repository holds the **Typescript React** `eslint` configuration for all projects inside the **@kwizapp** organization.

## Usage

### Installation

```bash
npm install @kwizapp/eslint-config-ts-react
```

**Note:** make sure you have a `.npmrc` with the following content:

```bash
@kwizapp:registry=https://npm.pkg.github.com/kwizapp
```

Otherwise `npm` will not know here to pull the package from.

### Peer Dependencies

Make sure your project has the following packages installed:

- prettier
- eslint
- eslint-config-prettier
- eslint-plugin-prettier
- eslint-plugin-react
- @typescript-eslint/eslint-plugin
- @typescript-eslint/parser

```shell
npm install --save-dev prettier eslint eslint-config-prettier eslint-plugin-prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-plugin-react
```

### Applying ESLint Rules

Create a `.eslintrc.js` file in the root of your project with the following content:

```js
module.exports = {
  extends: ["@kwizapp/eslint-config-ts-react"]
};
```

`eslint` will find this file on it's path

### Linting

Make sure you enable linting inside your editor.

**`npm scripts`**
You can use the following command to lint your project files. Add the following to your `package.json`.

```json
scripts": {
  "lint": "eslint \"{src,test}/**/*.{ts,tsx}\" --fix",
},
```

more information [here](https://eslint.org/)
