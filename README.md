reacted-form
===

Easily write forms in React.

# Install

```bash
npm install -s reacted-form
```

# Usage

Import form from one of your controller:

```js
import React from 'react';
import { Form, Email, Password } from 'reacted-form';

class MyComponent extends React.Component {

  submitHandler (e, values) {
    myLoginFunction(values.email, values.password):
  }

  render () {
    return (
      <Form onSubmit={ this.submitHandler.bind(this) }>
        <Email
          placeholder   =   "Your email"
          name          =   "email"
          required
        />
        <Password
          placeholder   =   "Your password"
          name          =   "password"
          required
        />
      </Form>
    )
  }
}
```
