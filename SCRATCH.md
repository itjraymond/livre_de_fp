# Scratch Pad - Expressing some ideas 

### 2021-02-28

Today I was reading additional info on Monads.  Specifcally the Reader Monad, Writer Monad and the
State Monad.  It turns out that this can also be thought as:

- Consumer Monad
- Supplier Monad
- Function Monad

The Consumer and Supplier Monad are slightly more general than the Reader and Writer Monad.
We shall use Reader/Writer Monad when we want to be explicit while using a Consumer/Supplier Monad 
can be used when the Reader/Writer Monad is not quite representative of the concept at hand.

The Function Monad is very generic and thus the State Monad shall be used when we really
want to express states changes.

Note, the above is not based on any literature (i.e. Reader Monad ~= Consumer Monad) hence it
may be total BS.
