# React Hook Cheatsheet
Don't remember which hook to use? Here's a quick reference sheet to go through all the options and understand the differences between each one. Below is a list of official  hooks (⚛️) as well as custom hooks (✴️). 

## Hooks

### Manage Component State

- ⚛️ [useState](https://react.dev/reference/react/useState)
   Read and update local values from a component
- ✴️ [useKeyedState](./useKeyedState)
   Read and update values from an individual item within a component

### Share Data Across Components

- ⚛️ [useContext](https://react.dev/reference/react/useContext)
   Read data shared across descendant components
- ✴️ [useStore](https://www.npmjs.com/package/use-store)
  Share data between components in different parts of the app
- ⚛️ [useRef](https://react.dev/reference/react/useRef#referencing-a-value-with-a-ref)
   Store data without triggering a component re-render

### Work With the DOM and External JS

- ⚛️ [useEffect](https://react.dev/reference/react/useEffect)
   Run side effects after the component has rendered
- ⚛️ [useLayoutEffect](https://react.dev/reference/react/useLayoutEffect)
   Run side effects *before* the browser paints the screen
- ⚛️ [useRef](https://react.dev/reference/react/useRef#manipulating-the-dom-with-a-ref)
   Access DOM elements directly

### Optimize Rendering

- ⚛️ [useMemo](https://react.dev/reference/react/useMemo)
   Recalculate a value only when dependencies change
- ⚛️ [useCallback](https://react.dev/reference/react/useCallback)
   Redefine a function only when dependencies change

