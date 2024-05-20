# `@signed/prettier-config`

> My personal [Prettier](https://prettier.io) config.

## Usage

**Install**:

```shell
pnpm add -D @signed/prettier-config
```

## Use as-is

**Edit `package.json`**:

```
{
  // ...
  "prettier": "@signed/prettier-config"
}
```

## Use as base configuration

To add e.g. the prettier tailwind plugin create `prettier.config.mjs`
as [local prettier configuration](https://prettier.io/docs/en/configuration.html) with

```javascript
import signed from '@signed/prettier-config'

const config = {
    ...signed,
    plugins: ['prettier-plugin-tailwindcss'],
}

export default config
```
