practice link : https://csbin.io/
Goes through the code line-by-line and runs/ ’executes’ each line - known as the thread of execution

Saves ‘data’ like strings and arrays so we can use that data later - in its memory

We can even save code (‘functions’)

```javascript
const num = 3; 
function multiplyBy2 (inputNumber){ 
	const result = inputNumber*2; 
	return result;
} 
const output = multiplyBy2(num); 
const newOutput = multiplyBy2(10);
```

In memory
num: 3
multiplyBy2: [function]
output: 

output = multiplyBy2(3)
																			local Memory
																			inputNumber: 3
																			result: 6
 return result

then locate the result and return it

newOutput => new execution context

Execution context

Created to run the code of a function - has 2 parts (we’ve already seen them!) 
- Thread of execution
- Memory

Call stack-
- JavaScript keeps track of what function is currently running (where’s the thread of execution) 
- Run a function 
- add to call stack 
- Finish running the function - JS removes it from call stack - Whatever is top of the call stack - that’s the function we’re currently running



