> The easiest way to use HashMap with a custom type as key is to derive Eq and Hash. We must also derive PartialEq.

```rust
    // ElephantSQL max 5 concurrent connection
    let pool = Pool::builder().max_size(5).build(manager)?;
```

### simple sub command
```rust
fn main() {
    let mut args = std::env::args();

    match (args.next(), args.next(), args.next()) {
        (_, Some(ref cmd), Some(ref x)) if cmd == "build" => build(x),
        (_, Some(ref cmd), Some(ref x)) if cmd == "run" => run(x),
        (_, Some(ref cmd), None) if cmd == "repl" => repl(),
        (_, Some(ref cmd), None) if cmd == "ide" => ide(),
        _ => {
            println!("Usage:");
            println!("  lark build <file> - compiles the given file");
            println!("  lark run <file>   - runs the given file");
            println!("  lark repl         - REPL/interactive mode");
            println!("  lark ide          - run the Lark languge server/IDE support");
        }
    }
}
```
