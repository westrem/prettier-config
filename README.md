# `@westrem/prettier-config`

Shared config for Prettier

# How to use

**Install**

```
yarn add --dev @westrem/prettier-config
```

**a) use with package.json**

```
// package.json
{
  ...,
  "prettier": "@westrem/prettier-config"
}
```

**b) use with .prettierrc.json**

```
// .prettierrc.json
"@westrem/prettier-config"
```

**Overrides**

Options above do not allow to extend the configuration. For that, you need to use following approach:

```
// .prettierrc.js
module.exports = {
  ...require("@westrem/prettier-config"),
  // custom overrides here
};
```

[More info on shared configurations](https://prettier.io/docs/en/configuration.html#sharing-configurations)