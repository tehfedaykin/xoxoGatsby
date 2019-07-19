## Let's get a Less Loader!

```bash
npm install --save less gatsby-plugin-less
```

// gatsby-config.js

```javascript
module.exports = {
  siteMetadata: {
    ...
  },
  plugins: [
    ...
    `gatsby-transformer-sharp`,
    `gatsby-plugin-less`,
    `gatsby-plugin-google-fonts`
  ],
}
```