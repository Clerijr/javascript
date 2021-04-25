#### Let's make those values interact!

Javascript needs more than informations to work, he need to know what to do with those informations. That's a lot of ways to do that, but the easiest and most common is using operators.

### Arithmetic

Those are the simplest and 'straightest' forward operators: 

- `-` Subtraction
- `+` Addition
- `*` Multiplication
- `/` Division
- `%` Remainder
- `=` Assignment

>ps.1: Javascript can convert a string to a number simply by using the Addition or Subtraction operators(the last one will try to convert the string to a negative number): <pre>let thirty = "30"<br>console.log(typeof thirty)  //string<br>console.log(typeof +thirty) //number
</pre>

>ps.2: We don't need to only use expressions like `a = a + b` if we want to change a variable's value. Javascript is smart enough to shorten those expressions and let we use the assignment operator together with another and make something like that: `a += b`

### Logical

There is 3 main types of Logical operators in Javascript, Unary(One value), Binary(Two values) and Ternary(Three values). They're strongly related to Boolean values, because if you're evaluating some value with them, you probably expect if your evaluation is `True` or `False`.

##### Unary
- <b>typeof</b>
    Show the evaluated value's type: `typeof "Javascript" //string`
- <b>Logical not</b>(`!`)
    Takes a true value as false and vice versa: `!true = false`
- <b>Increment and Decrement</b>(`--` and `++`)
    Add or subtract one from the value. If the operator comes before the value, it'll operate, then will return the new value. If the operator comes after, it will return the actual value, and then will operate:
    <pre>let twenty = 20, ten = 10<br>console.log(++20) //21<br>console.log(10--) //10</pre>
- <b>delete</b>
    Attempt to delete a value, returning true if the value is deleted and false if not, but doesn't work with functions or variables. Mostly used to delete object properties or array items.
    <pre>let myObj = {first: 1, second: "2", third: 3.0}<br>delete myObj.second<br>console.log(myObj) // { first: 1, third: 3 }</pre>
- <b>void</b>
    (This one is kinda weird i think) The void operator has the only purpose to return `undefined`. A link built like this won't do nothing because its linked to `undefined`: <pre><div align="center">`<a href="javascript:void(0)">This link does nothing</a>`</div></pre>

    
    
