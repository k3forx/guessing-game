# guessing_game

## Setting Up a New Project

```bash
❯ cargo new guessing_game

❯ cd guessing_game
```

- `Cargo.toml`

```toml
[package]
name = "guessing_game"
version = "0.1.0"
edition = "2018"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
```

## Processing a Guess

The first part of the guessing game program will ask for user input, process that input, and check that the input is in the expected form.

- `src/main.rs`

```rust
use std::io;

fn main() {
    println!("Guess the number!");

    println!("Please input your guess.");

    let mut guess = String::new();

    io::stdin()
        .read_line(&mut guess)
        .expect("Failed to read line");

    println!("You guessed: {}", guess);
}
```

### Storing Values with Variables

- The `::` syntax in the `::new` line indicates that `new` is an associated function of the `String` type. Some languages call this a _static method_.

- `.read_line(&mut guess)` calls the `read_line` method on the standard input handle to get input from the user. We’re also passing one argument to `read_line: &mut guess`.

### Handling Potential Failure with the Result Type

### Printing Values with println! Placeholders

### Testing the First Part

## Generating a Secret Number

## Comparing the Guess to the Secret Number

## Allowing Multiple Guesses with Looping

## Summary
