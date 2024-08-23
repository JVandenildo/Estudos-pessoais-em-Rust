# Studies in Rust

> [!IMPORTANT]
> This repository is for Rust algorithm/syntax testing.

Rust is a programming language focused on performance, safety, and concurrency. It accomplishes these goals without having a garbage collector.  
Its syntax is similar to C++, but Rust offers better memory safety while maintaining high performance.  
Originally created by [Graydon Hoare](https://github.com/graydon) on Mozilla Research, with contributions from [Brendan Eich](https://en.wikipedia.org/wiki/Brendan_Eich) (JavaScript's creator).  
Some IDEs for coding in Rust are:

- [Visual Studio Code](https://code.visualstudio.com/);
  - For having support for Rust via popular plugins, like "rust-analyzer".
- [RustRover](https://www.jetbrains.com/rust/);
  - A dedicated IDE for Rust development by JetBrains.
- [Vim](https://www.vim.org/);
- [Emacs](https://www.gnu.org/software/emacs/).

`Rust REPL` is an interactive shell in which is possible to write and test Rust snippets in real-time. It is not written in Rust, and do not require to be compiled. It is available via third-party tool such as `evcxr-repl`.

## Table of content

1. [Naming conventions](#naming-conventions);
2. [Installing Rust and Cargo](#installing-rust-and-cargo);
3. [References](#references).
   1. [References from internet articles](#references-from-internet-articles);
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
3. [roadmap.sh/rust](https://roadmap.sh/rust);
4. [app.daily.dev/tags/rust?ref=roadmapsh](https://app.daily.dev/tags/rust?ref=roadmapsh).

### References from internet articles

1. [doc.rust-lang.org/stable/rust-by-example/index.html](https://doc.rust-lang.org/stable/rust-by-example/index.html).

### References from videos

1. [Tutorial on Rust](https://youtu.be/T_KrYLW4jw8) from [@TechWithTim](https://www.youtube.com/@TechWithTim);
2. [Tutorial on VSCode with Rust](https://youtu.be/jvnZr7bJUfU) from [@doggodotrs](https://www.youtube.com/@doggodotrs);
3. "[Rust Installation, Hello World, Hello Cargo - Full Crash Rust Tutorial for Beginners](https://youtu.be/R33h77nrMqc?si=k01OHbuAwTHRpd3a)" do canal [@francescociulla](https://www.youtube.com/@francescociulla);
4. Playlist "[Convince your boss to use Rust](https://youtube.com/playlist?list=PLZaoyhMXgBzqkaLKR8HHWZaASMvW4gRtZ&si=M42726r8XPanN8ps)" do canal [@NoBoilerplate](https://www.youtube.com/@NoBoilerplate);
5. "[Rust in 100 seconds](https://youtu.be/5C_HPTJg5ek)" do canal [@Fireship](https://www.youtube.com/@Fireship).
