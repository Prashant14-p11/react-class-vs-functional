# react-class-vs-functional
# Class-Based Components
Use class keyword and extend React.Component.

Must include a render() method.

Can hold state using this.state.

Lifecycle methods like componentDidMount(), componentDidUpdate() are available.


class Welcome extends React.Component {
  constructor(props) {
    super(props);
    this.state = { message: 'Hello from class component' };
  }

  render() {
    return <h1>{this.state.message}</h1>;
  }
}


# Functional Components
Simple functions that return JSX.

-Initially stateless, but now can use hooks (like useState, useEffect) to manage state and side effects.

import React, { useState } from 'react';

function Welcome() {
  const [message, setMessage] = useState('Hello from functional component');

  return <h1>{message}</h1>;
}


