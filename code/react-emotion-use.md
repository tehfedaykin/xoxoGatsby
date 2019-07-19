## Use Emotion

```javascript
import styled from 'react-emotion'

const NavItem = styled('div')`
  background: #b8b365;
 `

const RightNav = () => {
  return (
    <NavItem>
      <Link className="nav-link" to="/">{' '}home{' '}</Link>
    </NavItem>
  )
}
 ```