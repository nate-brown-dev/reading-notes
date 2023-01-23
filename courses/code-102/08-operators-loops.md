# Code 102 Reading 8

## Operators and loops

> @non-technical-friend wrote:  
> Please help me understand assignment operators. I’m totally lost.

To get a good handle on this you have to remember back to your algebra days.

> But I took Algebra 1 in 1997!

So did I, but it’s coming back to me slowly.

According to MDN, an *expression* is *a valid unit of code that resolves to a value*.

While the program will run simple mathematical calculations like 2+2, it won’t save the result unless you tell it to, such as by using an assignment operator.

`2 + 2` runs but doesn’t do anything

however

``` javascript
let x;
x = 2 + 2;
```

assigns value of `2 + 2` to `x`

> What’s the difference between operators and operands?

The *operands* are the inputs used by the expression (x, 2, 2)

The *operators* are the mathematical/logic symbols that determine the relationship between the inputs.

Operators have *precedence* in code just like they have precedence in regular math / P-E-MD-AS.

> Some of these operators look familiar but other ones don’t seem to make any sense! Help!

JavaScript has both *binary* and *unary* operators.

Normal math symbols are examples of binary operators. All binary operators in JS are “infix” which means they go between the operands.

Unary operators are different! A unary expression has only one operand, so the operator has to go either before or after it (can’t be infix). Unary operators are either *prefix* (most of them) or *postfix* (++ and --)

An example of a unary expression is `x++` (increment x)

> What kinds of operators do I need to know about?

Only 2 kinds, assignment operators and comparison operators.

Assignment operators take the value of the right operand, and *assign* it to the left operand.

for example `x = f()` *assigns* the return of function f() to x

> What happens if I chain together a bunch of operators?

Chaining operators is bad practice and may break your code!

``` javascript
let x;
x = y = f();
```

The expression evaluates left to right but the assignment operator assigns the right side of the expression to the left side, so even if f() is valid, it attempts to assign the undeclared variable *y* to *x* before returning f()

> I’m totally lost again!

That’s ok, you’ll get it eventually. We’re going to push on to comparison operators.

Comparison operators determine if expressions are true or false.

For example, the comparison operator `!=` produces a result of `true` if the operands are not equal

if `const x = 7`, a function expression `x == 5` would return `false`

> Thanks a lot!

You aren’t done yet! We still have to talk about loops.

> What’s a loop?

A loop is a way to execute an expression more than once.

We only care about 2 kinds of loops right now, `for` and `while`.

The `for` loop has a conditional statement for which the loop repeats itself until the statement returns `false`.  This could go on indefinitely, or it could have an increment counter that causes it to run a certain number of times.

A `while` loop evaluates as long as its condition is ‘true’.

> It sounds like they do exactly the same thing!

They make a lot more sense when you write them out in JavaScript syntax.

Here's a `for` loop:

``` javascript
for (let x = 1; x < 10; x++) {
    console.log(x);
}
```

Now we can break down the components of the `for` loop

for (initialization; condition; increment) {
    statement;
}

1. initialization = what value does the loop start with?
2. condition = is the current value of the loop true or false? (if false, the loop breaks)
3. increment = if the current state is true, apply some change to the current value (ie increment, add 1)
4. statement = do something, then restart the loop

And here's a `while` loop:

``` javascript
let x = 1;
while (x != 10) {
    x++;
    console.log(x);
}
```

Both of these loops do exactly the same thing!

[Go back home](/reading-notes/)
