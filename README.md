# @la-ots/stylelint-config

Standard rules for CSS and SASS using [Stylelint](https://stylelint.io/) implemented as a common configuration.

## Installation

```bash
npm install --save-dev @la-ots/stylelint-config
```

### Configure settings

Create `.stylelintrc.js` file with the following content:

```javascript
module.exports = {
  extends: "@la-ots/stylelint-config",
};
```

### Using with Prettier

If you're using this plugin with [Prettier](https://prettier.io), add "prettier" at the end of your extends list:

```javascript
module.exports = {
  extends: ["@la-ots/stylelint-config", "stylelint-config-prettier"],
  rules: {
    // your custom rules
  },
};
```

## Running linters

Add the following scripts to your `package.json`:

```javascript
{
  "scripts": {
    "lint-css": "stylelint *.{css,scss}"
  }
}
```

Execute scripts:

```bash
npm run lint-css
```
