# Algebraic Traits

 - Currencies.jl doesn't work with promotion system
 - Need algebraic traits to deal with physical units better

## problem 1: how to handle identity elements?

 - Trouble is: some structures have only a left-identity or a right-identity
 - but most have both, and it's just a single identity
 - want to make it easy to specify that there is a single identity
 - but also want to preserve the generality of both left- and right-identities

## solution: LeftIdentity and RightIdentity as separate traits, and Identity as both

 - but in general, we should prefer higher granularity over lower granularity
 - macros/functions can be made to simplify defining a large number of methods

## problem 2: how close is close enough?

 - do floating points count as a field?
 - they have some major exceptions, like `NaN` or `Inf`
 - but this is computing... are they an appropriate field anyway?

## another problem

 - there are so many different kinds of invertibility!
 - only a few of them are practical
 - gotta figure out a good basis and build on that

## trait dispatch

 - use a library?
 - make sure to actually dispatch, or things are weird
