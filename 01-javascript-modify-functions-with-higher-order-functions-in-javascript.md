[Video Link](https://egghead.io/lessons/javascript-modify-functions-with-higher-order-functions-in-javascript)

# 01. Modify Functions with Higher Order Functions

**A higher order function does at least one of two things. Sometimes both**

1. Accepts a functon as an argument
2. Returns a new function 



For demonstration let's make a higher order function called ```<withCount>```. This will take a function(fn) as an argument. So that it logs how many times the function has been called.

```javascript
const withCount = fn => {

}
```

Inside of the function we'll make a count variable. Then we will return a new function that uses the spread operator to gather the arguements assigned to it.

Inside the body of our return we'll log the count variable while icrementing it. Then we;ll reutn the results of the function that has been called with the spread arguements.

```javascript
const withCount = fn => {
  let count = 0

  return (...args) => {
    console.log(`Call count: ${++count}`)
    return fn(...args)
  }
}
```




# Personal Take
Nothing really this course get more clear and concise as it moves on

# Resources
[Kyle Shevlin Blog Post On Higher Order Functions](https://kyleshevlin.com/just-enough-fp-higher-order-functions)

