 # Refactoring
 ## What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

**how do we know if a function is pure or not**
- It returns the same result if given the same arguments (it is also referred as deterministic)

- It does not cause any observable side effects.

#### impure function :uses a global object that was not passed as a parameter to the function.
also Any function that relies on a random number generator cannot be pure

##### Pure functions benefits:
The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
- Given a parameter A → expect the function to return value B
- Given a parameter C → expect the function to return value D

### When data is immutable:
 its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
In Javascript we commonly use the for loop. This next for statement has some mutable variables.
