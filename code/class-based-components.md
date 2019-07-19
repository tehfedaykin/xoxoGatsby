### Class-Based Components

```javascript
class Navigation extends React.Component {
  constructor(props) {
    super(props);
      this.toggleNavbar = this.toggleNavbar.bind(this);
      this.state = { collapsed: true,};
  }

  toggleNavbar() {
    this.setState({ collapsed: !this.state.collapsed});
  }
  render() {
    const DDMenu = 'navbar-collapse' + (this.state.collapsed ? ' collapse' : '')
    return (
      <button onClick={this.toggleNavbar}>
        <span className="navbar-toggler-icon"></span>
      </button>
      <div className={DDMenu} id="navbarSupportedContent">
        ... my nav stuff
      </div>
    )
  }
}

export default Navigation
```

Use these when you care about managing state
