# Building a React App

###Simplest way to define a component:

```
import React, { Component } from 'react'

 {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

###More advanced Component

```class App extends React.Component {
    // fires before mounting
    constructor(props) {

        // Super makes THIS COMPONENT refer to THIS COMPONENT
        super(props);

        // set local state (sometimes this is where the axios call would be???)
        this.state = {
            date: new Date()
        };

    }
//the above is required to be able to call the {this.state...} below
    render() {
        return (
            <h1>
                It is {this.state.date.toLocaleTimeString()}.
            </h1>
        )
    }

}
```

* Adding local state to class.

###That Fun Extension cheatsheet

⋅⋅⋅ | --- | --- |
| rcc→ | class component skeleton |
| rrc→ | class component skeleton with react-redux connect |
|rccp→ | class component skeleton with prop types after the class|
|rcjc→ | class component skeleton without import and default export lines |
|rcfc→ | class component skeleton that contains all the lifecycle |methods|
|rwwd→ | class component without import statements|
|rpc→ | class pure component skeleton with prop types after the class|
|rsc→ | stateless component skeleton|
|rscp→ | stateless component with prop types skeleton|
|rpt→ | empty propTypes declaration|
|rdp→ | empty defaultProps declaration|
|con→ | class default constructor with props|
|conc→ | class default constructor with props and context|

###Sources:
https://ihatetomatoes.net/react-tutorial-for-beginners/
https://reactjs.org/docs/components-and-props.html
