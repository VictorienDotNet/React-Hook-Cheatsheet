# React Hook Cheatsheet
Don't remember which hook to use? Here's a quick reference sheet to go through all the options and understand the differences between each one.

## Hooks

### Manage Component State

- **useState**
   Read and update local values from a component
- **useKeyedState**
   Read and update values from an individual item within a component

### Share Data Across Components

- **useContext**
   Read data shared across descendant components
- **useStore**
   Share data between components in different parts of the app
- **useRef**
   Store data without triggering a component re-render

### Work With the DOM and External JS

- **useEffect**
   Run side effects after the component has rendered
- **useLayoutEffect**
   Run side effects *before* the browser paints the screen
- **useRef**
   Access DOM elements directly

### Optimize Rendering

- **useMemo**
   Recalculate a value only when dependencies change
- **useCallback**
   Redefine a function only when dependencies change

