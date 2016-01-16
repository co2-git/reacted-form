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
import Form from 'reacted-form';

class MyComponent extends React.Component {

  submitHandler (e, values) {
    myLoginFunction(values.email, values.password):
  }

  render () {
    return (
      <Form name="login" onSubmit={ this.submitHandler.bind(this) }>
        <input
          type          =   "email"
          placeholder   =   "Your email"
          name          =   "email"
          required
        />
        <input
          type          =   "password"
          placeholder   =   "Your password"
          name          =   "password"
          required
        />
      </Form>
    )
  }
}
```
