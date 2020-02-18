```javascript
import React from 'react'

const Message = (props) => {
 console.log('I am rendering with props', props)
 return (
   <p>{props.message}</p>
 )
}
```

![Component Anatomy](../../assets/react-component-anatomy.png)

![Component with Internal Function](../../assets/react-component-internal-func.png)
