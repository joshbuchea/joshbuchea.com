---
layout: post
title: React Cheatsheet
category: React
---

# ReactJS

## ES6 Class

```jsx
class Component extends Component {
  render() {
    return <div>Hello {this.props.name}</div>;
  }
}
```

```
ReactDOM.render(<Component name="John" />, mountNode);
```

## Stateless Function

```
function Component(props) {
  return <div>Hello {props.name}</div>;
}
```

```
ReactDOM.render(<Component name="John" />, mountNode);
```

## Nesting

```
class UserAvatar extends React.Component {...}
class UserProfile extends React.Component {...}
```

```
function Info(props) {
  return (
    <div>
      <UserAvatar src={props.avatar} />
      <UserProfile username={props.username} />
    </div>
  );
}
```

## State & Props

### ES6 Class

```
<MyComponent fullscreen={true} />
```

```
// props
this.props.fullscreen //=> true

// state
this.setState({ username: 'johndoe' });
this.replaceState({ ... });
this.state.username //=> 'johndoe'
```

```
render: function () {
  return (
    <div className={this.props.fullscreen ? 'full' : ''}>
      Welcome, {this.state.username}
    </div>
  );
}
```

### Stateless

```
<MyComponent fullscreen={true} />
```

```
// props
props.fullscreen //=> true
```

```
function MyComponent (props) {
  return (
    <div className={props.fullscreen ? 'full' : ''}>
      Welcome!
    </div>
  );
}
```
