### Functional Components

```javascript
function MyComponent(props) {
  return <div>{props.name}</div>
}
```

"props" are properties supplied to React components

```javascript
class Index extends React.Component {
  render() {
    const image = siteUrl + get(this, 'props.data.headshotImage.sizes.src');

    return (
      <Layout location={this.props.location} title={siteTitle}>
        <Hero headerImage={this.props.data.headerImage}
          heading="Jennifer Wadella"
          text="Often described as a force of nature, 
          lol jk Jennifer sucks at coding" />
        </div>
      </Layout>
    )
  }
}
```
