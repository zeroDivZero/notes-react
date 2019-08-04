# VIRTUAL DOM (VDOM)

Ideal representation of UI, kept in memory and synced with real DOM by lib such as **ReactDOM**. This process is called *reconciliation*.

Enables declarative API: inform React of UI state, and it makes DOM match it. Abstracts out attribute manipulation, event handling, and manual DOM updating.

More pattern than tech, can mean different things. In React usually associated with **elements** (smallest building blocks, objects representing UI). React also uses internal objects *fibers* to hold additional info about component tree; may also be considered part of VDOM.

## Shadow DOM

**Shadow DOM** is browser tech designed to scope vars and CSS in web components. VDOM is implemented by JS libs on top of browser APIs. *Not same.*

## Fiber

Reconciliation engine in React 16. Main goal is to enable incremental rendering of VDOM.
