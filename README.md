# boot-unplugin

[![NPM version](https://img.shields.io/npm/v/boot-unplugin?color=a1b858&label=)](https://www.npmjs.com/package/boot-unplugin)

Starter template for [unplugin](https://github.com/unjs/unplugin).

## Template Usage

To use this template, clone it down using:

```bash
npx degit kirklin/boot-unplugin my-unplugin
```

And do a global replace of `boot-unplugin` with your plugin name.

Then you can start developing your unplugin 🔥

To test your plugin, run: `pnpm run dev`
To release a new version, run: `pnpm run release`

## Install

```bash
npm i boot-unplugin
```

<details>
<summary>Vite</summary><br>

```ts
// vite.config.ts
import Starter from "boot-unplugin/vite";

export default defineConfig({
  plugins: [
    Starter({ /* options */ }),
  ],
});
```

Example: [`playground/`](./playground/)

<br></details>

<details>
<summary>Rollup</summary><br>

```ts
// rollup.config.js
import Starter from "boot-unplugin/rollup";

export default {
  plugins: [
    Starter({ /* options */ }),
  ],
};
```

<br></details>


<details>
<summary>Webpack</summary><br>

```ts
// webpack.config.js
module.exports = {
  /* ... */
  plugins: [
    require("boot-unplugin/webpack")({ /* options */ })
  ]
};
```

<br></details>

<details>
<summary>Nuxt</summary><br>

```ts
// nuxt.config.js
export default {
  buildModules: [
    ["boot-unplugin/nuxt", { /* options */ }],
  ],
};
```

> This module works for both Nuxt 2 and [Nuxt Vite](https://github.com/nuxt/vite)

<br></details>

<details>
<summary>Vue CLI</summary><br>

```ts
// vue.config.js
module.exports = {
  configureWebpack: {
    plugins: [
      require("boot-unplugin/webpack")({ /* options */ }),
    ],
  },
};
```

<br></details>

<details>
<summary>esbuild</summary><br>

```ts
// esbuild.config.js
import { build } from "esbuild";
import Starter from "boot-unplugin/esbuild";

build({
  plugins: [Starter()],
});
```

<br></details>


## License

[MIT](./LICENSE) License © 2022 [Kirk Lin](https://github.com/kirklin)
