# React_Interview_Question

#1.What is a generator function in JavaScript? How does it work?
A generator function is a special type of function that can be paused and resumed. It is defined using the function* syntax and uses the yield keyword to yield values. Generators are useful for implementing iterators.

2.Explain closures in JavaScript:
A closure is a function that has access to its own scope, the scope of the outer function, and the global scope. It allows functions to retain access to variables from their enclosing scope even after the outer function has finished executing.

3.What are higher-order components in React?
Higher-order components (HOCs) are functions that take a component and return a new component with added functionality. They allow for code reuse and logic sharing across multiple components.

4.Explain the difference between state and props in React:
State is an internal data storage that is local to a component and can change over time. Props are external inputs passed to a component from its parent, and they are immutable.

5.What is a Callback function?
A callback function is a function passed as an argument to another function. It is executed after the completion of the function it was passed to, allowing for asynchronous operations.

6.Explain the spread operator in JavaScript:
The spread operator (...) allows for the expansion of iterable elements (like arrays or objects) into individual elements. It is used for array and object manipulation.

7.What is the difference between a shallow copy and a deep copy? How do you create each type in JavaScript?
A shallow copy copies only the first level of an object, while a deep copy copies all levels. Shallow copy can be created using Object.assign() or the spread operator. Deep copy can be created using JSON.parse(JSON.stringify(object)) or a recursive function.

8.What is the Virtual DOM in React, and how does it help?
The Virtual DOM is an in-memory representation of the real DOM. React uses it to optimize and batch updates, improving performance by minimizing direct DOM manipulations.

9.What are hooks in React? Name some commonly used hooks:
Hooks are functions that let you use state and other React features in functional components. Commonly used hooks include useState, useEffect, useContext, useReducer, and useRef.

10.Explain useMemo and React.memo, and describe the differences between them:
useMemo is a hook that memoizes the result of a function. React.memo is a higher-order component that memoizes a component, preventing unnecessary re-renders. useMemo is used within components, while React.memo is used to wrap components.

11.What are the use cases for useCallback and useMemo? Provide examples:
useCallback is used to memoize functions, preventing them from being recreated on every render. useMemo is used to memoize values. Example:

javascript
const memoizedCallback = useCallback(() => {
    doSomething(a, b);
}, [a, b]);

const memoizedValue = useMemo(() => computeExpensiveValue(a, b), [a, 
