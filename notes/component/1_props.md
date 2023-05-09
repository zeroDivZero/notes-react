# PROPS

Args accepted by component to change behavior or appearance. Data flows *down* component tree: **one-way** data flow. State can be passed from parent to child as props.

```jsx
const Header = ({ title }) => {
  return <h1>{ title ? title: "Develop. Preview. Ship. 🚀" }</h1>;
}

const HomePage = () => {
  return (
    <div>
      <Header title="React 💙" />
      <Header />
    </div>
  );
}
```

Args passed as obj to component function. Use object destructuring to explicitly name values.

In JSX, use `{}` for JS expression.

## `key`

If using array to define list component, React needs to uniquely identify array items to update elements in DOM. Pass identifier to `key`:

```jsx
const HomePage = () => {
  const names = ['Ada Lovelace', 'Grace Hopper', 'Margaret Hamilton'];

  return (
    <div>
      <Header title="React 💙" />

      <ul>
        {names.map(name => (
          <li key={name}>{name}</li>
        ))}
      </ul>
    </div>
  );
}
```

Typically should use unique identifier instead of value as key, since values could have duplicates.
