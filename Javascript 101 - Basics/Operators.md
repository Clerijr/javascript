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

>ps.1: Javascript can convert a string to a number simply by using the Addition or Subtraction operators(the last one will try to convert the string to a negative number) and this make those operators work as unary too: <pre>let thirty = "30"<br>console.log(typeof thirty)  //string<br>console.log(typeof +thirty) //number
</pre>


>ps.2: We don't need to only use expressions like `a = a + b` if we want to change a variable's value. Javascript is smart enough to shorten those expressions and let we use the assignment operator together with another and make something like that: `a += b`

### Logical

There is 3 main types of Logical operators in Javascript, Unary(One value), Binary(Two values) and Ternary(Three values). They're strongly related to Boolean values, because if you're evaluating some value with them, you probably expect if your evaluation is `True` or `False`.

#### Unary

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
    (This one is kinda weird i think) The void operator has the only purpose to return `undefined`. A link built like this won't do nothing because its linked to `undefined`: <pre>`<a href="javascript:void(0)">This link does nothing</a>`</pre>

#### Binary

- <b>Bitwise</b>
    Theres some operators know as bitwise, but due to my lack of info i'll write this topic another time.

- <b>Comparison and Deep Comparison</b>(`==`and`===`)
    They're used to compare if two variables/values are equal. The difference between them is that `==` compare the values and `===` compare values and types:
     <pre>
    let someNumber = 10
    let someString = '10'
    someNumber == someString // true
    someNumber === someString // false
    </pre>
- <b>Not equal value and not equal value nor type</b>(`!=`and`!==`)
    Works as opposite from the last ones, evaluating if two values are different:
    <pre>
    let someNumber = 10
    let someString = '10'
    someNumber != someString // false
    someNumber !== someString // true
    </pre>
- <b>Greater than, Less than, Greater than or equal to, Less than or equal to</b>(`>`,`<`,`>=`and`<=`)
    Okay this one you probably know from math so i'll not explain because i'm too lazy and too sleepy right now to write everything...
    <pre>
    let bigNumber = 10
    let smallNumber = 5
    bigNumber > smallNumber // true
    bigNumber < smallNumber // false
    bigNumber >= smallNumber +5 // true
    bigNumber <= smallNumber // false
    </pre>
- <b>Logical AND</b>(`&&`)
    Returns true if both expressions and/or values are true:
    <pre>
    let twentyFive = 25
    let thirtyTwo = 32
    console.log(twentyFive < thirtyTwo && thirtyTwo > twentyFive) // true
    console.log(twentyFive > thirtyTwo && thirtyTwo > twentyFive) // false
    </pre>
    
- <b>Logical OR</b>(`||`)
    Returns true if one of the expressions and/or values is true:
    <pre>
    let twentyFive = 25
    let thirtyTwo = 32
    console.log(twentyFive > thirtyTwo || thirtyTwo > twentyFive) // true
    console.log(twentyFive > thirtyTwo || thirtyTwo < twentyFive) // false
    </pre>
##### Short Circuit
A really cool resource in Javascript is the short circuit with those logical expressions, works like this: As `&&` and `||` need **two** expressions to operate, Js will evaluate the first expression and if it's enough to give our answer, he won't read the other. Example:
<pre>
twentyFive < thirtyTwo || thirtyTwo < twentyFive // The first(left) expression is true, the second will be skipped
twentyFive > thirtyTwo && thirtyTwo > twentyFive // Same here, don't need to evaluate the second if the first is enough to return false
</pre>

Knowing that we can work with expressions using undefined parameters, because if its undefined its false, if there's a value it is true:
<pre>
let userInput                               // declaring a variable without value
let characterName = userInput || 'John Doe' // characterName == 'John Doe'
userInput = 'Bob Builder'                   // assigning a value to our variable
characterName = userInput || 'John Doe'     // With userInput defined, we name our character correctly!
</pre>

#### Ternary

The ternary operator is kinda a shorten version of the `if` conditional. He'll evaluate the first expression and if it returns `true`, the second expression will be executed, if it's `false`, the third expression will be:
<pre>
let bigNumber = 10
let smallNumber = 5
bigNumber > smallNumber ? console.log("This'll be executed") : console.log("This'll be ignored")
</pre>

<div style="display:flex;justify-content:space-between"><a href="README.md">&#8592;&nbsp;Variables and Values</a><a href="README.md">HOME</a><a href="Operators.md">Conditionals&nbsp;&#8594;</a></div>