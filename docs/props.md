<h1>Part 4. Props</h1>

Props are like a mixture of HTML attributes and JavaScript function parameters. Props are necessary when you need to transfer data between the parent component and the child component.

The following example has two components: **myApp** and **greeting**. myApp-component represents the parent component and greeting-component represents the child component.

The props of the greeting-component contain two properties: name and lastName.

```typescript
// greeting.tsx
import React from 'react'

// set the required props
type GreetingProps = {
  name: string,
  lastName: string,
}

// use props like a params
const Greeting: React.FC<GreetingProps> = ({ name, lastName }) => {
  return (
    <div>
      <p>{ `Hello, ${name} ${lastName}!` }</p>
    </div>
  )
}

export default Greeting

```

greeting-component usage with props ``<Greeting name='Jaakko' lastName='Kulta' />``

```typescript
//myApp.tsx
import React, { useState } from 'react'
import Greeting from './greeting';

type MyAppProps = {

}

const MyApp: React.FC<MyAppProps> = () => {

  // useState hooks for name & lastName
  const [name, setName] = useState<string>('');
  const [lastName, setLastName] = useState<string>('');

  return (
    <div>

      {/* input for name */}
      <label>
        name:
        <input
          type='text'
          {/* set input value to value of name */}
          value={name}
          {/* using onChange event to set name, every time whent value of input has changed */}
          onChange={ (event) => setName(event.target.value) }
        />
      </label>

      {/* input for lastName */}
      <label>
        last name:
        <input
          type='text'
          value={lastName}
          onChange={ (event) => setLastName(event.target.value) }
        />
      </label>

      {/* dispaly greetings */}
      {/* here we use greeting-component props like a HTML attributes */}
      <Greeting name={name} lastName={lastName} />

    </div>
  )
}

export default MyApp

```

## [<-- BACK TO PART 3 (HOOKS)](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/usestate.md) ...... [GO TO PART 5 (ROUTER) -->](https://github.com/JoniRinta-Kahila/portfolioproject/blob/master/docs/router.md)

