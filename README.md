# @martijnhols/eslint-config

This package includes my shareable ESLint configuration.

## Usage

To use this configuration first install this package:

```sh
yarn add -D @martijnhols/eslint-config
```

Then add this to your `package.json`:

```json
    "eslintConfig": {
        "extends": "@martijnhols/eslint-config"
    },
```

The `eslintConfig` property is used by create-react-app, IDE extensions and seems to be [standard](https://eslint.org/docs/user-guide/configuring).

## Customization

Customization is not recommended. Please consider making a pull request to this
package instead.

To apply custom rules remove the eslint configuration from your `package.json`, then create a file named `.eslintrc.json` with following contents in the root folder of your project:

```json
{
  "extends": "@martijnhols/eslint-config"
}
```

That's it! You can override the settings by editing the `.eslintrc.json` file. Learn more about [configuring ESLint](http://eslint.org/docs/user-guide/configuring) on the ESLint website.

## Options

These options can be enabled/disabled using env variables.

`CODE_STYLE` Enable or disable code style rules in eslint. These rules are
automatically fixable, so this can be run in a precommit hook with `--fix`.
