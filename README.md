# JavaScript - Parentheses vs. Brackets vs. Curly Braces

## When to use each:

### Parentheses
* Function calls 
  ```
  let str = "Hello"
  str = str.toLowerCase()
  // str has the value: "hello"
  ```
  ```
  let myArray = [1, 2, 3, 4, 5]
  newArray = myArray.map(number => number * 2)
  // newArray has the value: [2, 4, 6, 8, 10] 
  ```
* Surrounding parameters in an arrow function
  ```
  let myArray = [1, 2, 3, 4, 5]
  // surrounding the number parameter in parentheses
  myArray.map((number) => number * 2)
  // When there is only one parameter, it is optional to surround the parameter in parentheses. The below is acceptable as well
  myArray.map(number => number * 2)
  ```
* Surrounding conditional statements
  ```
  if(1 > 0) {
    console.log("1 is greater than 0")
  }
  // Prints "1 is greater than 0" to the console
  ```
* Grouping to enforce order of operations
  ```
  let number = ((1 + 2) * 4) - 1
  // number has the value: 11 
  ```

### Brackets
* Denoting an array
  ```
  let myArray = [1, 2, 3, 4, 5]
  ```
* Indexing into an array to get a value
  ```
  let myArray = [2, 10, 5, 4, 9]
  let myValue = myArray[3]
  // myValue has the value: 4
  ```
* Accessing the property of an object
  ```
  let myObject = {
    name: "Ricky",
    age: 35,
    job: "Junior Analyst"
  }

  console.log(myObject["name"])
  // Prints "Ricky" to the console

  console.log(myObject["age"])
  // Prints 35 to the console

  console.log(myObject["job"])
  // Prints "Junior Analyst" to the console

  // NOTE: dot notation is also acceptable to access the property of an object
  ```

### Curly Braces
* Declaring object literals
  ```
  let myObj = {
    name: "Jane",
    age: 40,
    job: "Senior Analyst"
  }
  ```
* Enclosing blocks of code (loops, function definitions, conditional blocks, etc)
  ```
  for (var i = 0; i < 5; i++>) {
    console.log(i)
  }
  ```
  ```
  function myFunc() {
    console.log("This is my function")
  }
  ```
  ```
  if(1 > 0) {
    console.log("1 is greater than 0")
  }
  ```
