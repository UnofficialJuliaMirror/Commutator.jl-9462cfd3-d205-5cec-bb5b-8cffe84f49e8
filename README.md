# Commutator

This package provides the function `commutator!` that calculates the
[commutator](https://en.wikipedia.org/wiki/Commutator)
`[A, B]` of two ring elements `A`, `B`. That is,


    commutator!(alpha, A, B, beta, C)

evaluates in-place to

    C = beta * C + alpha * (A * B - B * A)


Typically, `A, B, C` are subclasses of `AbstractMatrix`, and `beta` and `alpha`
are a `Number`.