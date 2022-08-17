# @navify/swiftlint-config

Shared SwiftLint config used in Navify and Jigra projects. This must be used with the [`swiftlint` wrapper](https://github.com/navify/swiftlint) for npm projects.

## Usage

1. Install the `@navify/swiftlint` wrapper by following [these instructions](https://github.com/navify/swiftlint#usage).
1. Remove existing `.swiftlint.yml` file, if present.
1. Install the config in your project.

    ```
    npm install -D @navify/swiftlint-config
    ```

1. Configure the swiftlint wrapper by adding a `@navify/swiftlint` key at the root of your project's `package.json`.

    ```
    "@navify/swiftlint": "@navify/swiftlint-config",
    ```

    > Alternatively, to override options, you can create a `swiftlint.config.js` file:
    >
    > ```javascript
    > module.exports = {
    >   ...require('@navify/swiftlint-config'),
    >
    >   // override options here
    > };
    > ```
    >
    > It might be worth creating a PR to this config repo first, though! We'd love to discuss changes. :blue_heart:
