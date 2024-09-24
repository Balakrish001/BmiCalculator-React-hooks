# Effect Hook 

- Persisting Application data
  - Local Storage
- Storing values in Local Storage
  - Using Effect Hook
- Tips for using Effect Hook
  - Multiple Effects
  - Dependency Array
# React Hooks and useEffect

## 1. Persisting Data While Using React Hooks

### 1.1 Storing Values in Local Storage
In `useEffect`, we have access to the updated state values, so we write the logic for storing values inside it.

### 1.2 Getting Values from Local Storage
Once after getting the values from Local Storage, provide them as the initial values for the `useState` hook.

## 2. Tips for Using the Effect Hook

### 2.1 Using Multiple `useEffect`s to Separate Concerns
Just like `useState`, you can also use multiple `useEffect`s to separate unrelated logic into different effects based on what it is doing.

### 2.2 Optimizing Performance by Skipping Effects
In some cases, executing the effect after every render creates a performance problem. It can be optimized by skipping the effect when it is not required.

The `useEffect` accepts another argument called the Dependency Array, using which we can control the execution of the effect.

**Syntax:**
```javascript
useEffect(effect, [var1, var2, ...]);
