# Symbols

- `m!` | indicates a **macro** call
- `$(x),*` | match repetition in macros by example
- `#[attr]` | outer **attribute**
- `![attr]` | inner **attribute**
- `'a` | **lifetime parameter**, often seen as `&'a T` 
- `a::b` | **namespace path**
- `'a: loop` | Loop label
- `x;` | **Statement** terminator, otherwise **expressions**
- `x?` | Early return **error propagation**



# Number Literals

- `98_222` | Decimal
- `0xff` | Hex
- `0o77` | Octal
- `0b1111_0000` | binary
- `b'A'` | Byte (u8 only)



# Keywords

- `x as u32` | Primitive **cast** (may truncate etc)

- `break x;` | Exit loop and yield `x` as value of loop

- `continue;` | Continue to next loop iteration

- `const X` | Define a **constant**

- `extern crate` | Declares dependency on external crate

- `fn f() -> T {}` | Function definition

- `x: fn f()` | Function pointers

- `let x;` | Bind a variable

- `loop {}` | Loop unconditionally

- `match m { ... }` | Initiate **pattern matching**

- `mod m {} ` | Define a **module**

- `static X` | **Global variable** with 'static' lifetime




# Referencing

- `&x` | immutable **borrow**

- `&T` | immutable **reference**

- `&mut x` | mutable **borrow**

- `&mut T` | mutable **reference**

- `*const T` | immutable **raw pointer type**

- `*mut T` | mutable**raw pointer type**

- `*x` | **dereferencing**


# built-in Types

- `S { x: y }` | **initialize** field x of **struct** S with value y
- `S { x }` | **initialize** field x of **struct** S with value x
- `[T; n]` | **Array** with n copies of T's Default
- `[x; n]` | **Array** with n copies of x
- `[x, y, z]` | **Array** with given elements
- `x[0]` | **Indexing** on collection
- `x[..]` | **slice-like** indexing on collection
- `x[a..]` | **slice-like** indexing on collection
- `x[..b]` | **slice-like** indexing on collection
- `x[a..b]` | **slice-like** indexing on collection
- `a..b` | Right exclusive **range**
- `a..=b` | Right inclusive **range**
- `x.i` | **Member access**
- `x.0` | **Tuple access**







# Generics

TODO