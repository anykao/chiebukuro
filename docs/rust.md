> The easiest way to use HashMap with a custom type as key is to derive Eq and Hash. We must also derive PartialEq.

```rust
    // ElephantSQL max 5 concurrent connection
    let pool = Pool::builder().max_size(5).build(manager)?;
```
