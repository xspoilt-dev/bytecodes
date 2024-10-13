# **Python bytecodes** *along with their meaning.*

| **INSTRUCTION**          | **MEANING**                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `POP_TOP`                | Removes the top of the stack.                                                |
| `ROT_TWO`                | Swaps the two top-most stack items.                                          |
| `ROT_THREE`              | Rotates the top three stack items (top goes to third position).              |
| `DUP_TOP`                | Duplicates the top stack item.                                               |
| `DUP_TOP_TWO`            | Duplicates the top two stack items.                                          |
| `NOP`                    | Does nothing (no operation).                                                 |
| `UNARY_POSITIVE`         | Applies the unary `+` operator to the top of the stack.                      |
| `UNARY_NEGATIVE`         | Applies the unary `-` operator to the top of the stack.                      |
| `UNARY_NOT`              | Inverts the truth value of the top stack item.                               |
| `UNARY_INVERT`           | Bitwise inversion (`~`) of the top stack item.                               |
| `BINARY_ADD`             | Adds the top two stack items.                                                |
| `BINARY_SUBTRACT`        | Subtracts the second stack item from the top item.                           |
| `BINARY_MULTIPLY`        | Multiplies the top two stack items.                                          |
| `BINARY_DIVIDE`          | Divides the second stack item by the top item.                               |
| `BINARY_MODULO`          | Computes the remainder (modulus) of the top two stack items.                 |
| `BINARY_POWER`           | Raises the second stack item to the power of the top item.                   |
| `BINARY_AND`             | Performs bitwise AND on the top two stack items.                             |
| `BINARY_OR`              | Performs bitwise OR on the top two stack items.                              |
| `BINARY_XOR`             | Performs bitwise XOR on the top two stack items.                             |
| `LOAD_FAST`              | Loads a local variable onto the stack.                                       |
| `STORE_FAST`             | Stores the top stack item in a local variable.                               |
| `LOAD_CONST`             | Loads a constant onto the stack.                                             |
| `RETURN_VALUE`           | Returns the top stack item as the function result.                           |
| `JUMP_FORWARD`           | Unconditionally jumps forward by a specified number of bytes.                |
| `JUMP_IF_TRUE_OR_POP`    | Jumps if the top stack item is true, otherwise pops the top item.            |
| `JUMP_IF_FALSE_OR_POP`   | Jumps if the top stack item is false, otherwise pops the top item.           |
| `COMPARE_OP`             | Performs comparison operations (e.g., <, <=, ==, !=, >, >=).                 |
| `CALL_FUNCTION`          | Calls a function with the specified number of arguments.                     |
| `MAKE_FUNCTION`          | Creates a function object.                                                   |
| `BUILD_LIST`             | Creates a list from a specified number of top stack items.                   |
| `BUILD_TUPLE`            | Creates a tuple from a specified number of top stack items.                  |
| `BUILD_SET`              | Creates a set from a specified number of top stack items.                    |
| `BUILD_MAP`              | Creates a dictionary from key-value pairs on the stack.                      |
| `IMPORT_NAME`            | Imports a module by name and pushes it to the stack.                         |
| `LOAD_ATTR`              | Loads an attribute from an object and pushes it to the stack.                |
| `STORE_ATTR`             | Stores the top stack item as an attribute of an object.                      |
| `LOAD_GLOBAL`            | Loads a global variable onto the stack.                                      |
| `STORE_GLOBAL`           | Stores the top stack item in a global variable.                              |
| `RAISE_VARARGS`          | Raises an exception using the arguments on the stack.                        |
| `SETUP_LOOP`             | Begins a loop block (used for loops like `for` and `while`).                 |
| `BREAK_LOOP`             | Breaks out of the current loop.                                              |
| `CONTINUE_LOOP`          | Continues to the next iteration of a loop.                                   |
| `POP_BLOCK`              | Pops a block from the block stack (used in try/except/finally and loops).    |
| `END_FINALLY`            | Ends the execution of a `finally` block.                                     |
| `WITH_CLEANUP`           | Cleans up after the `with` statement.                                        |
| `LOAD_CLOSURE`           | Loads a closure variable onto the stack.                                     |
| `MAKE_CLOSURE`           | Creates a closure and pushes it onto the stack.                              |
| `LOAD_DEREF`             | Loads a value from a closure cell.                                           |
| `STORE_DEREF`            | Stores a value into a closure cell.                                          |
| `SETUP_WITH`             | Prepares the stack for the `with` statement.                                 |
| `EXTENDED_ARG`           | Extends the argument for an opcode by adding more significant bits.          |
| `FORMAT_VALUE`           | Formats a value using formatting specifiers.                                 |
| `BUILD_CONST_KEY_MAP`    | Builds a dictionary using a list of keys and values.                         |
| `UNPACK_SEQUENCE`        | Unpacks a sequence into individual stack items.                              |
| `UNPACK_EX`              | Unpacks a sequence with specified variable-length items.                     |
| `GET_ITER`               | Gets an iterator for a sequence.                                             |
| `FOR_ITER`               | Iterates over an iterable (for loops).                                       |
| `YIELD_VALUE`            | Yields a value from a generator function.                                    |
| `LOAD_BUILD_CLASS`       | Loads the `__build_class__` function for class creation.                     |
| `SET_ADD`                | Adds an element to a set (while constructing a set).                         |
| `MAP_ADD`                | Adds an item to a dictionary (while constructing a dict).                    |
| `LIST_APPEND`            | Appends an item to a list (while constructing a list).                       |
| `JUMP_ABSOLUTE`          | Unconditionally jumps to a specific instruction.                             |
| `LOAD_METHOD`            | Loads a method for bound method calls.                                       |
| `CALL_METHOD`            | Calls a method with the arguments on the stack.                              |
| `GET_AWAITABLE`          | Gets an awaitable object from a coroutine.                                   |
| `LOAD_ASSERTION_ERROR`   | Loads the `AssertionError` exception class.                                  |
| `SETUP_ASYNC_WITH`       | Prepares for an asynchronous `with` statement.                               |
| `BEFORE_ASYNC_WITH`      | Handles the setup before entering an async `with` block.                     |
| `END_ASYNC_FOR`          | Ends an asynchronous for loop.                                               |



> [!NOTE]  
> ****The Python bytecode set can change across different Python versions, so these instructions are reflective of Python 3.x versions.****
