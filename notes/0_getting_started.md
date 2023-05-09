# GETTING STARTED

## Create App

`npx`:

```sh
npx create-react-app my-app
```

`npm`:

```sh
npm init react-app my-app
```

`yarn`:

```sh
yarn create react-app my-app
```

## Run App

In project folder, with `npm`:

```sh
npm start
```

`yarn`:

```sh
yarn start
```

## Using unpkg.com

### Import

In HTML:

* **react**: core lib
* **react-dom**: provides DOM-specific methods

```html
<script src="https://unpkg.com/react@17/umd/react.development.js"></script>
<script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"></script>
```

### Add Babel (JS Compiler)

Browser doesn't understand JSX. Need to transform to JS.

```html
<script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
```

Then set script type to `jsx`:

```html
<script type="text/jsx">
  const app = document.getElementById('app');
  ReactDOM.render(<h1>Develop. Preview. Ship. 🚀</h1>, app);
</script>
```
