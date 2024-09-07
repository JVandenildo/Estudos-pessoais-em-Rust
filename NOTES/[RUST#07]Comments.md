# Comentários em Rust

Comentários são declarações que não são processadas no programa. Sendo um meio interessante para esclarecer algum ponto no código. Esse tipo de comentário é chamado de "comentário idiomático".  
Um exemplo de comentário em Rust:

```rust
// hello there
```

O Rust não possui suporte para comentários de múltiplas linhas, como em C++ ou JavaScript, o que tem que ser feito são múltiplos comentários de linhas únicas. Exemplo:

```rust
// Alguma coisa que precisa de comentário
// é tanto comentário que ocupa mais de uma linha
// ocupa três linhas! que coisa
```

Os comentários podem ser colocados no final de uma declaração. Exemplo:

```rust
fn main(){
    let lucky_number = 7; // o ainda é número da sorte?
}
```

Existe ainda o comentário de documentação.

## Referências

1. [doc.rust-lang.org/book/ch03-04-comments.html](https://doc.rust-lang.org/book/ch03-04-comments.html).

### Referências em artigos na web

### Referências em vídeos
