# Studies in Rust

Repository for C++ algorithm/syntax testing.

## Table of content

1. [Naming conventions](#naming-conventions);
2. [References](#references).

## Naming conventions

> [!INFO] INFO  
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
3. [Tutorial on Rust](https://youtu.be/T_KrYLW4jw8?si=ClI3lnU5kgE4kO46) from [@TechWithTim](https://www.youtube.com/@TechWithTim);
4. [Tutorial on VSCode with Rust](https://youtu.be/jvnZr7bJUfU?si=ZjpUwl-pvGJCwAaD) from [@doggodotrs](https://www.youtube.com/@doggodotrs).
