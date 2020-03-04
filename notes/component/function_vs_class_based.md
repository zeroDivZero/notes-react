# FUNCTION VS CLASS-BASED

## Function

```javascript
import React, { useState } from 'react'
import TitleEditor from './title-editor'

const StatefulFunctionComponent = () => {
 const [title, setTitle] = useState('Electrode Rocks!')

 const updateTitle = (title) => { setTitle(title) }

 return (
   <main>
     <h1>{title}</h1>
     <TitleEditor handleUpdate={updateTitle} />
   </main>
 )
}

export default StatefulFunctionComponent
```

## Class-based

```javascript
import React, { Component } from 'react'
import TitleEditor from './title-editor'

class StatefulComponent extends Component {
 constructor(props) {
   super(props)
   this.state = { title: 'Electrode Rocks!' }
   this.updateTitle = this.updateTitle.bind(this)
 }

 updateTitle = (title) => { this.setState({ title }) }

 render() {
   return (
     <main>
       <h1>{this.state.title}</h1>
       <TitleEditor handleUpdate={this.updateTitle} />
     </main>
   )
 }
}

export default StatefulComponent
```

## Verdict

Functional more declarative, less boilerplate code. With hooks, functional can do everything class-based can. Community moving toward functional. Recommended by React creator.
