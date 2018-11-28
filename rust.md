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