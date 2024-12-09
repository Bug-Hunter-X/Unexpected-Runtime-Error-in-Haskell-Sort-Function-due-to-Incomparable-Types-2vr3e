# Haskell Sorting Bug: Incomparable Types
This repository demonstrates a common yet subtle error in Haskell involving the sorting of lists with incomparable types. The `sort` function from `Data.List` requires all elements to be instances of the `Ord` typeclass, and attempting to sort a list containing elements with incompatible `Ord` instances results in a runtime error. 

**bug.hs** contains the buggy code, which compiles but throws a runtime error when trying to sort a list containing both integers and strings. 

**bugSolution.hs** provides a corrected version that uses a custom comparison function to handle heterogeneous data types, preventing the runtime error.  This solution demonstrates proper type handling and error prevention in Haskell.