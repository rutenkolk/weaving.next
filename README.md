# weaving.next



Weaving is to lambdas what threading is to s-expressions.

This library's purpose is to provide a set of simple function combinators to ease out the day-to-day wrangling of Clojure code.

Just like threading macros in Clojure end with an arrow, weaving functions end with |.

```clj
[weaving.next "0.1.0"]
```

[![Build Status](https://travis-ci.org/rutenkolk/weaving.next.svg?branch=master)](https://travis-ci.org/rutenkolk/weaving.next)
[![codecov](https://codecov.io/gh/rutenkolk/weaving.next/branch/master/graph/badge.svg)](https://codecov.io/gh/rutenkolk/weaving.next)
[![Clojars Project](https://img.shields.io/clojars/v/weaving.next.svg)](https://clojars.org/weaving.next)


Fork of TristeFigure's weaving library, which sadly, vanished.

## Usage

weaving:


    conditionals: if|, when|, or|, and| & not|.
    partialization: | & ||. On the model of -> and ->>,
        (| str "ABC") produces strings like "_ABC" while
        (|| str "ABC") produces strings like "ABC_".
    function arguments weaving: •|,
        ((•| + identity (constantly 1)) 2) yields 3.
    other control flow: tap| inspired by ruby.
    <-| : works like constantly.
    *|: works like juxt.
    juxtm|: works like juxt but accepts and returns a map.
    =|: (=| 2) is equivalent to #(= % 2).
    ->|: works like comp but in a reverse, sane order (the same as ->).
    apply|.
    args|.
    call.
    in|.


## License

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
