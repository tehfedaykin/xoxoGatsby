## Transform Markdown

[Gatsby-transformer-remark](https://www.gatsbyjs.org/packages/gatsby-transformer-remark/?=gatsby-transformer-remark)

```bash
npm install --save gatsby-transformer-remark
```

// gatsby-config.js

```javascript
plugins: [
  {
    resolve: `gatsby-transformer-remark`,
    options: {
      commonmark: true, // CommonMark mode (default: true)
      footnotes: true, // Footnotes mode (default: true)
      pedantic: true, // Pedantic mode (default: true)
      gfm: true, // GitHub Flavored Markdown mode (default: true)
      // Plugins configs
      plugins: [],
    },
  },
],
```