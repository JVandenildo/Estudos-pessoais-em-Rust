# Variáveis e Tipos de Dados

No Rust, as variáveis são declaradas a palavra-chave `let`. Todas as variáveis são imutáveis por padrão, o que significa que uma vez que o valor for vinculado a variável, ele não pode ser alterado. Caso queira declarar uma variável mutável, a palavra-chave `mut` é usada. Por exemplo:

```rust
let x = 5;
let mut y = 5;
```

A variável `x` é imutável, enquanto `y` é mutável.  
Por padrão do Rust, variáveis tem o escopo dentro do bloco que estão, além de ter suporte há diferentes tipos de atributos de variável.

## Sumário

1. [Enums](#enums);
2. [Referências](#referências).
   1. [Referências em artigo da internet](#referências-em-artigos-da-internet);
   2. [Referências em vídeos](#referências-em-vídeos).

## Enums

Um enum (abreviação de _enumeration_) é um tipo de dado customizado que permite ao programador definir um tipo apenas anumerando (listando um por um) todas as suas possíveis variações. No Rust, caso alguma coisa for de um conjunto de possibilidades (`Pedra`, `Papel` ou `Tesoura`, por exemplo), talvez seja mais apropriado representar esse tipo de dado com um enum (`enum RPsChoice { Rock, Paper Scissors }`).  
Uma instância de um `enum` pode ter uma e somente uma das variantes declaradas do enum em qualquer momento. Diferente de enumerações em outras linguagens, variantes no Rust não são restritas a um tipo de dado único. Quando um `enum` é definido, é possível decidir para cada um de suas variantes se terão ou não algum tipo de dado diferente, é possível também permitir deixar tipos em quantidades diferentes. É possível colocar estruturas e outros enums em uma variante.

## Referências

1. [roadmap.sh/rust](https://roadmap.sh/rust).

### Referências em artigos da internet

1. [rust-book.cs.brown.edu/ch03-01-variables-and-mutability.html](https://rust-book.cs.brown.edu/ch03-01-variables-and-mutability.html);
2. [rust-book.cs.brown.edu/ch03-02-data-types.html](https://rust-book.cs.brown.edu/ch03-02-data-types.html);
3. [rust-book.cs.brown.edu/ch06-01-defining-an-enum.html](https://rust-book.cs.brown.edu/ch06-01-defining-an-enum.html).

### Referências em vídeos
