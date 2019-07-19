## Gatsby Background Image

```bash
npm install --save gatsby-background-image
```

```javascript
import BackgroundImage from "gatsby-background-image"

const Layout = ({ children }) => {
  const data = useStaticQuery(graphql`
    query SiteTitleQuery {
      desktop: file(relativePath: { eq: "background.jpg" }) {
        childImageSharp {
          fluid(quality: 90, maxWidth: 4160) {
            ...GatsbyImageSharpFluid_withWebp
          }
        }
      }
    }
  `)
  return (
    <BackgroundImage Tag="section"
      fluid={data.desktop.childImageSharp.fluid}
      backgroundColor={`#000000`}
    >
    {{children}}
    </BackgroundImage>
      )
}
```
