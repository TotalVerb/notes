# Algebraic Traits

 - Currencies.jl doesn't work with promotion system
 - Need algebraic traits to deal with physical units better

## problem 1: how to handle identity elements?

 - Trouble is: some structures have only a left-identity or a right-identity
 - but most have both, and it's just a single identity
 - want to make it easy to specify that there is a single identity
 - but also want to preserve the generality of both left- and right-identities
