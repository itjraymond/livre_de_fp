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

Note, above is not based on any literature (i.e. Reader Monad ~= Consumer Monad) hence it
may be total BS.

#### Idea 

Come up with some Java demonstration and show that the language is limited when doing FP but
feasible if using existing libraries or come up with your own.

For instance, can you "mimic" algebraic data type?

public interface Option<A>

public class Some<A> extends Option
public class None<A> extends Option

Then implement map, flatmap, unit? etc.

Also, see if you can do:
public interface Monad<A>

In which case the Monad is only a contextual computation that hides a certain value of type A.

How about `lift` functions?  You need to understand those as well.

