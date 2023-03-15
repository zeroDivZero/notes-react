# `useState`

For functional component, use **hook** `useState`.

```javascript
import React, { useState } from 'react'

const Counter = () => {
  const [count, setCount] = useState(0)
  const increment = () => { setCount(count + 1) }
  return (
    <button onClick={increment}>
      Clicked {count} times
    </button>
  )
}
```

Cannot be used in class-based component.
