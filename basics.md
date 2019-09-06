## Essentials

Haskell has `type inference` - No need to label every piece of code with type info. Type system can figure out
a lot about things.

+ Interactive mode on haskell can be activated by typing in `ghci`. You can load up functions `:l myFunction` defined  in a `.hs` script. If a change is made to a function it can be reloaded in the repl via the command `:r`.
+ `/=` means not equal to.
+ Functions are written in prefix usually with the params separated via spaces, no paranthesis.
Eg: 
```
ghci> succ 8
9
```

Function application has the highest precedence!

If a function takes two arguments, it can be written in `infix` notation, the name of the function should be surrounded by backticks.

```
ghci> 4 `max` 5
5
```

+ The else part in haskell's `if-else` block is mandatory.
+ If statement is an `expression` - something that returns a value. That's why the if statement
is an expression.

+ An `apostrophe` can be used in a funciton name, usually it's symbolic of a non-lazy function.
+ A function name cannot begin with an upper case character.
+ Functions that don't take any params are called `definitions`.


## Lists

+ Lists are `homogeneous`, they can only store data of one type.
+ `let` can be used to define a name in ghci
+ strings are just list of characters so list functions can be used on them.
+ `++` concatenates two lists. Caveat: Haskell iterates over all elements of the list on the LHS.
+ `:` Cons operator, adds something to the front of a list.
+ List actually looks like `1:2:3:[]`
+ Getting element out of a list use the `!!` operator. `[1, 2, 3] !! 1`
+ If a list is a 2D list or a 3D list all the sub lists should be of the same type.
+ Basic ops on a list: `head, tail, init, last, length, reverse`
+ null checks if a list is empty
+ `take` and `drop` take an int and a list has args and do what you'd expect with em.
