# unit-3-code-analysis-practice

Using markdown, identify what the following code block does and explain how the `forEach` function works.

```js
function forEach(arr, action) {
  for (let i = 0; i < arr.length; i++) {
    action(arr[i]);
  }
}

forEach(['a', 'b', 'c'], console.log);
```

**Guiding Questions:**
* What does the code do (what does it print? are any variable reassigned? etc...)
* What are the expected data types for each of the parameters?
* When the function is invoked, what value are provided as arguments?
* How does `forEach` use the provided arguments?

**Key Terms to use**: parameters, arguments, invoke/invocation, iterate, "element of the array", increment,  

<hr>

Your explanation here...

The code snippet above will log `a`, `b`, and `c` to the console seperately. First, the function `forEach` is declared with two parameters: `arr` and `action`. Then, a for loop is implemented, with the purpose of *iterating* through each element in `arr`. In the following code block, `action(arr[i])` will make it so that the `action` parameter can access each element in `arr` through their respective **index** represented by `i`. Finally, when invoking the function `forEach()`, the `arr` argument `['a', 'b', 'c']` will have its elements logged to the console, as a result of the `action` argument, `console.log`, the *function that accesses and logs each element* onto the console.
