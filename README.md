# Studies in Rust

Repository for Rust algorithm/syntax testing.

## Table of content

1. [Naming conventions](#naming-conventions);
2. [Installing Rust and Cargo](#installing-rust-and-cargo);
3. [References](#references).
   1. [References from articles across web](#references-from-articles-across-web);
   2. [References from videos](#references-from-videos).

## Installing Rust and Cargo

In order to install Rust, go to the official website [rust-lang.org](https://www.rust-lang.org) and download the appropriate installation file for the operating system. It will install `rustup`, which is the preferred tool for installing, updating and managing the core Rust tooling.  
It is worth noticing that, to create executables, is necessary a linker on the machine, such as 'GCC'. Otherwise, errors will be faced when trying to run `rustc` or `cargo`. This is one necessary thing that `rustup` doesn't install.

> [!TIP]
> In doubt go to [doc.rust-lang.org/stable/book/ch01-01-installation.html](https://doc.rust-lang.org/stable/book/ch01-01-installation.html).

Rust is updatable at any time by running `rustup update` the terminal.

## Naming conventions

> [!TIP]  
> Here are some conventions, for more details go to the [documentation](https://rust-lang.github.io/api-guidelines/naming.html).

| Item            | Convention             |
| --------------- | ---------------------- |
| Modules         | `snake_case`           |
| Functions       | `snake_case`           |
| Methods         | `snake_case`           |
| Macros          | `snake_case`           |
| Local variables | `snake_case`           |
| Statics         | `SCREAMING_SNAKE_CASE` |
| Constants       | `SCREAMING_SNAKE_CASE` |
| Enum variants   | `UpperCamelCase`       |

Some important points to have in mind:

- In `UpperCamelCase`, acronyms and contractions of compound words count as one word;
- In `snake_case` or `SCREAMING_SNAKE_CASE`, a word should never consist of a single letter unless it is the last word;
- Crate names should not use `-rs` or `-rust` as a suffix or prefix.

## References

1. [Rust official website](https://www.rust-lang.org/);
2. [Rust documentation](https://doc.rust-lang.org/stable/book/index.html);
3. [roadmap.sh/rust](https://roadmap.sh/rust).

### References from articles across web

### References from videos

1. [Tutorial on Rust](https://youtu.be/T_KrYLW4jw8) from [@TechWithTim](https://www.youtube.com/@TechWithTim);
2. [Tutorial on VSCode with Rust](https://youtu.be/jvnZr7bJUfU) from [@doggodotrs](https://www.youtube.com/@doggodotrs).
