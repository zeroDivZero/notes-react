# `useState`

For functional component (not class-based), use **hook** `useState`.

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

State initiated and stored within component. Can pass it to children components as prop, but update logic should be kept locally.
