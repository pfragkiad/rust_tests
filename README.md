# rust_tests
RUST tests

Main tutorial site: https://doc.rust-lang.org/rust-by-example/hello.html

# Initialize and run project

To initialize and run project run:
```sh
cargo new rust_tutorial
cd rust_tutorial
cargo run
```


# Hello world program

```rust
fn main() {
    println!("Hello, world!");
}
```

Sample declaration of variables with print corresponding statements:

```rust
fn main() {
    // Integer types
    let i: i32 = 42;
    println!("i: {} is an i32", i);

    // Floating-point types
    let f: f32 = 3.14;
    println!("f: {} is an f32", f);

    // Boolean type
    let b: bool = true;
    println!("b: {} is a bool", b);

    // Character type
    let c: char = 'a';
    println!("c: {} is a char", c);

    // String type
    let s: &str = "Hello, world!";
    println!("s: {} is a string", s);

    // Array type
    let a: [i32; 3] = [1, 2, 3];
    println!("a: {:?} is an array of i32", a);

    // Tuple type
    let t: (i32, &str) = (1, "one");
    println!("t: {:?} is a tuple", t);
    
    // Function pointer
    let func_pointer: fn() = main;
    println!("func_pointer: {:?} is a function pointer", func_pointer);
    
    // Struct type
    //derive allows the the {:?} format specifier
    #[derive(Debug)]
    struct Point {
        x: i32,
        y: i32,
    }
    let p = Point { x: 1, y: 2 };
    println!("p: {:?} is a struct of Point", p);
    
    // Enum type
    //derive allows the the {:?} format specifier
    #[derive(Debug)]
    enum Color {
        Red,
        Green,
        Blue,
    }
    let color = Color::Red;
    println!("color: {:?} is an Enum of Color", color);
}

```
