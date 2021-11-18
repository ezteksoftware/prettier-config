# A shared Prettier config

## Installation

Using npm

```
npm install @eztek/prettier-config --save-dev
```

Using yarn

```
yarn add @eztek/prettier-config --dev
```

## Usage

Add a key in your **package.json** file.

```
"prettier": "@eztek/prettier-config"
```

If you don't want to use package.json, you can use any of the supported extensions to export a string, e.g. `.prettierrc.json`:

```
"@eztek/prettier-config"
```

Note: This method does not offer a way to extend the configuration to overwrite some properties from the shared configuration. If you need to do that, import the file in a `.prettierrc.js` file and export the modifications, e.g:

```
module.exports = {
  ...require("@eztek/prettier-config"),
  semi: false
};
```
