# sloth

- a lazy dynamically-typed functional language built on Julia
- uses Julia parser and runs on top of Julia
- everything lazy by default
- can call eager Julia functions
- can be called from eager Julia functions
- tail call elimination (of course)
- no max stack depth ever
- graph reduction

first steps: build it as a lisp (see SExpressions.jl) and then extend it to use Julia syntax

## haskell ideas

 - possible parenthesis-free function calls by using macrocall syntax
 - i.e. `@f x y z` to mean `f(x, y, z)`?
 - different approach to metaprogramming needed
