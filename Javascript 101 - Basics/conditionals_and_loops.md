### <div align="center">Conditionals and Loops</div>
<div align="center"><i><b>For</b> each room we need some windows, and a door <b>If</b> theres none</i></div>
</div>

---

#### IF

When you find yourself into a code with 2 possible paths, you need to specify how the code will deal with those situations. **IF** condition **A** is true, do something, if don't, continue in another way(we can improve this and build more conditions, but let's simplify by now).


>The code block looks like this:
&nbsp;
if(boolean value or expression){
    //Do this if True
}else{
    //Do this if False
}
//Continue the code
&nbsp;
================================
We can shorten the expression by not using the **else** block, we can also avoid de braces, like that:
&nbsp;
if(boolean value or expression) console.log("Do that");
&nbsp;

---

#### FOR

Now we're dealing with a situation that demands some repetition, it's a *Loop*. The **FOR** structure is composed by 4 parts:

1. A variable that's gonna work as starting point(commonly used `let i = 0`)
2. The condition to end the loop, based in the initial variable
3. Incrementing or Decrementing the variable
4. The for body itself

>The block can be written like this:
&nbsp;
for (let i = 0; i <= 5; i++){
console.log(i)
}
&nbsp;
The output will be that:
0
1
2
3
4
5



<p align="center"><a href="operators.md">&#8592;&nbsp;Operators</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="README.md">HOME</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="../Fantastic%20Objects/objects_and_arrays.md">Objects and Arrays&nbsp;&#8594;</a></p>
