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
    let lucky_number = 7; // o 7 ainda é número da sorte?
}
```

Existe ainda o comentário de documentação.

## Sumário

1. [Comentário de documentação](#comentário-de-documentação);
   1. [Comentário de documentação como testes](#comentários-de-documentação-como-testes);
   2. [Comentando itens contidos](#comentando-itens-contidos).
2. [Referências].
   1. [Referências em artigos da web](#referências-em-artigos-na-web);
   2. [Referências em vídeos](#referências-em-vídeos).

## Comentário de documentação

Usado principalmente para documentar os pacotes criados em Rust, os comentários de documentação geram uma documentação HTML. Esse tipo de comentário é usado para programadores interessados em como usar o pacote (ou _crate_, como é chamado em Rust).  
Os comentários de documentação usam três barras, `///`, e tem suporte a notação Markdown para formatação de texto. A documentação é inserida logo antes do item que está documentando.  
Exemplo:

````rust
/// Soma um ao número inserido
///
/// # Exemplos
/// ```
/// let arg = 5;
/// let answer = my_crate::add_one(arg);
///
/// assert_eq!(6, answer);
pub fn add_one(x: i32) -> i32 {
    x + 1;
}
````

A documentação HTML é gerada rodando o comando `cargo doc`. Esse comando executa a ferramenta `rustdoc` distribuída com Rust e coloca a documentação em HTML no diretório "target/doc".  
Por conveniência, executar `cargo doc --open` builda o HTML para a documentação do crate atual (assim como a documentação para todos as dependências do crate) e abre o resultado no navegador.

### Seções comumente usadas

Além da seção `# Examples` para listar exemplos, usada no exemplo acima, também são usados:

- **Panics**: os cenários que a função documentada poderia retornar o erro;
- **Errors**: caso a função retorne um `Result`, descreve os tipos de erros que pode ocorrer e quais condições podem causar esses erros;
- **Safety**: caso a função seja `unsafe`, deveria ter uma seção documentando o por quê da função ser insegura.

### Comentários de documentação como testes

Adicionar exemplos de código na documentação pode ajudar a demonstrar como usar a biblioteca/crate, e fazendo isso tem um bônus adicional: rodar `cargo test` executa os exemplos de código da documentação.  
É interessante sabe que caso o exemplo da documentação esteja diferente do código que esteja exemplificando, o `cargo test` retornará um erro.

### Comentando itens contidos

O estilo de comentário de documentação `//!` adiciona documentação ao item que contém o comentário invés do item que segue o comentário. É usado normalmente dentro do arquivo root do pacote/crate ("src/lib.rs", por convenção) ou dentro de um módulo para documentar o crate ou módulo como um todo.  
Exemplo:

```rust
//! # Meu crate
//!
//! `meu_crate` é uma coleção de utilitários que fazem
//! algo útil

/// Adiciona um ao número inserido
/// --continua--
```

Vale notar que não tem código depois da última linha que começa com `//!`. Esses comentários estão documentando o item que contém o comentário.  
Quando a linha `cargo doc --open` for executada, esses comentários aparecerão na página de frente da documentação do `my_crate`.

## Referências

1. [doc.rust-lang.org/book/ch03-04-comments.html](https://doc.rust-lang.org/book/ch03-04-comments.html).

### Referências em artigos na web

### Referências em vídeos
