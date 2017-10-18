# eslint-plugin-ante

Standard linting rules for ESLint, suitable for all JavaScript projects.

## Installation

We recommend installing `eslint` and `eslint-plugin-ante` locally within your project:

```sh
# Install eslint if it is not already installed.
$ yarn add --dev eslint

# Install this plugin.
$ yarn add --dev eslint-plugin-ante
```

## Configuration

Within your ESLint configuration file (e.g: **.eslintrc.json**), add an entry to the "plugins" section:

```json
{
  "plugins": [
    "eslint-plugin-ante"
  ]
}
```

### Shareable Configurations

#### Recommended

The `recommended` configuration enforces a significant subset of the core non-stylistic rules listed at [ESLint: Rules](https://eslint.org/docs/rules/), covering the "Possible Errors", "Best Practices", "Variables", and "ECMAScript 6" sections. It is highly recommended to use this *in conjunction with* the `eslint:recommended` configuration provided natively by ESLint, as this configuration *does not include* those rules.

To use this configuration, add an entry to your ESLint configuration's `extends` section:

```json
{
  "extends": [
    "eslint:recommended",
    "plugin:ante/recommended"
  ]
}
```

#### Style

The `style` configuration enforces a set of stylistic conventions using the core rules described at [ESLint: Rules: Stylistic Issues](https://eslint.org/docs/rules/#stylistic-issues). These are not included in the `recommended` configuration above because some of the choices are highly subjective. We recommend using this configuration for new projects, or projects where **a convention** is desired rather than **a particular convention**, although any of the default rules provided in this configuration may be overridden in your project's `rules` section.

To use this configuration, add an entry to your ESLint configuration's `extends` section:

```json
{
  "extends": [
    "plugin:ante/style"
  ]
}
```

#### Possible Errors

The `possible-errors` configuration enforces a significant subset of the core rules described at [ESLint: Rules: Possible Errors](https://eslint.org/docs/rules/#possible-errors).

To use this configuration, add an entry to your ESLint configuration's `extends` section:

```json
{
  "extends": [
    "plugin:ante/possible-errors"
  ]
}
```

#### Best Practices

The `best-practices` configuration enforces a significant subset of the core rules described at [ESLint: Rules: Best Practices](https://eslint.org/docs/rules/#best-practices).

To use this configuration, add an entry to your ESLint configuration's `extends` section:

```json
{
  "extends": [
    "plugin:ante/best-practices"
  ]
}
```

#### ECMAScript 6

The `es6` configuration enforces a significant subset of the core rules described at [ESLint: Rules: ECMAScript 6](https://eslint.org/docs/rules/#ecmascript-6).

To use this configuration, add an entry to your ESLint configuration's `extends` section:

```json
{
  "extends": [
    "plugin:ante/es6"
  ]
}
```

#### Variables

The `variables` configuration enforces a significant subset of the core rules described at [ESLint: Rules: Variables](https://eslint.org/docs/rules/#variables).

To use this configuration, add an entry to your ESLint configuration's `extends` section:

```json
{
  "extends": [
    "plugin:ante/variables"
  ]
}
```

# License

eslint-plugin-ante is licensed under the [MIT License](http://www.opensource.org/licenses/mit-license.php).
