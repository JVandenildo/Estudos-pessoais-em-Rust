# Funções no Rust

Em Rust, as funções são declaradas usando a palavra-chave `fn`. Cada função pode receber um conjunto de variáveis de entrada com seus tipos específicos. O corpo de uma função é contido dentro de chaves `{}`.  
Diferente de outras linguagens, no Rust, não é necessário terminar a última declaração em um bloco com um ponto-e-vírgula `;`.  
Exemplo de função que retorna implicitamente:

```rust
fn add(one: i32, two, i32) -> i32 { one + two }
```

Essa função recebe os parâmetros `one` e `two` do tipo `i32` e retorna um inteiro também do tipo `i32` que é o resultado de `one + two`.  
Rust também possui a palavra-chave `return` para retornar um dado valor, dessa maneira:

```rust
fn add(one: i32, two: i32) -> i32{ return one + two; }
```

Usando uma declaração de retorno ou usar uma declaração de retorno implícito acaba sendo uma questão de gosto.

## Referências

1. [roadmap.sh/rust](https://roadmap.sh/rust).

### Referências em artigos da internet

1. [https://rust-book.cs.brown.edu/ch03-03-how-functions-work.html](https://rust-book.cs.brown.edu/ch03-03-how-functions-work.html).

### Referências em vídeos
