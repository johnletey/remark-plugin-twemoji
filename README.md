# remark-plugin-twemoji

Remark plugin to replace your emoji with [twemoji](https://github.com/twitter/twemoji).

## Install

```bash
# npm
npm install remark-plugin-twemoji
# yarn
yarn add remark-plugin-twemoji
```

## Usage

This plugin accepts an `option` prop, valid options are listed [here](https://github.com/twitter/twemoji#object-as-parameter).

1. [Next.js](https://nextjs.org/) Site

```js
// next.config.js
const withMDX = require("@next/mdx")({
  options: {
    remarkPlugins: [require("remark-plugin-twemoji")],
  },
});
module.exports = withMDX();
```

2. [Gatsby](https://www.gatsbyjs.org/) Site

```js
// gatsby-config.js
module.exports = {
  plugins: [
    {
      resolve: `gatsby-plugin-mdx`,
      options: {
        remarkPlugins: [require(`remark-plugin-twemoji`)],
      },
    },
  ],
};
```

---

[![MIT](https://img.shields.io/badge/license-MIT-0a0a0a.svg?style=flat&colorA=0a0a0a)](LICENSE)
