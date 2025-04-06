# useKeyedState

Read and update values from an individual item within a component

## When to Use It

Use this method to update a specific part of a state object, particularly in situations where the `useState` hook cannot be used, such as within the `Array.map` function.

```javascript
const useKeyedValue = useKeyedState()
const [isHover, setHover] = useKeyedValue(`unique-key`, false)
```



## The Hook

````javascript
import { useReducer, useCallback } from "react"

function stateReducer(state, action) {
    const { key, value } = action
    return { ...state, [key]: value }
}

export function useKeyedState() {
    const [state, dispatch] = useReducer(stateReducer, {})

    return useCallback(
        (key, initialValue) => {
            return [
                state[key] ?? initialValue,
                (value) => dispatch({ key, value }),
            ]
        },
        [state]
    )
}

````

