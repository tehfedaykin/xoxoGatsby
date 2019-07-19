## Importing CSS & fonts

```bash
npm install --save less gatsby-plugin-less gatsby-plugin-google-fonts
```

// gatsby-browser.js

```javascript
require('./src/assets/css/gg.less')
```

// gatsby-config.js

```javascript
module.exports = {
  plugins: [
    ...
    `gatsby-transformer-sharp`,
    `gatsby-plugin-less`,
    {
      resolve: `gatsby-plugin-google-fonts`,
      options: { fonts: [`Montserrat\:100,300,400,700`] }
    }
  ]
}
```
