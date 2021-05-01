### <div align="center">Variables and Values</div>
<div align="center"><i>To build a house, we need some bricks. But it's gonna be clay or concrete?</i></div>
</div>

---

Probably the best place to start (assuming that you know all the history about ecmascript and stuff like this) is talking about variables.

>Remember a bit:
<div align="center">&nbsp;&nbsp;1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;&nbsp;&nbsp;1&nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;0&nbsp;&nbsp;1&nbsp;&nbsp;0</div>
<div align="center">128&nbsp;&nbsp;&nbsp;64&nbsp;&nbsp;32&nbsp;&nbsp;16&nbsp;&nbsp;8&nbsp;&nbsp;4&nbsp;&nbsp;2&nbsp;&nbsp;1</div>

>Those ones and zeros represent the number 146 in binary, each single digit is a 'bit' and when you say for example `let value = 146`, the interpreter will take the piece of memory where it's binary version is located, and 'make a bridge' between them, because now you got a value(146) and his binary version, both accessed by your new variable `value`.

####So, what is a variable?

When we invoke a value, the aplication can(or not) change it, for example:
><pre>let myVariable = 10 //now we got the value 10 assigned to our variable<br>myVariable += 1     //the value changed, now it appoint to 11 instead of 10</pre>

This happens because we can't have all the values at the same time, that's gonna consume all our memory, so we address only the values that we want, using variables that can(or not) discard a value and pick another.

Those variables can be declarated using `let`, `var`or `const`, the last one can't be changed. We're gonna see the proper difference between them later.

####Going back to values

We already got and good idea about variables, but what about the Values? What about their particularities?

Those values can be divided by some types:
1. Number
    - Integers (`100`)
    - Fractionals (`100.00`)
    - Scientific Notation (`2.996e6`)
2. Special Numbers
    - Infinity
    - -Infinity
    - NaN(Not a Number)
3. Strings
     - Everything insite a pair of quotes(`'`), double quotes(`"`) or backticks(`` ` ``), are considered a string. Of course we got some variations, like escaping a string with `\n` or inserting a variable using template literals(Strings built using backticks) with `${myVariable}`
4. Booleans
    - True
    - False

5. Null and Undefined
    - Those values are interchangeable, the simplest example of them is declaring a variable without a value assigned to it(`let noValue`).



<p align="center"><a href="README.md">HOME</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="operators.md">Operators&nbsp;&#10140;</a></p>