# Memory safety e Zero-Cost Abstractions

"_Memory safety_" é assegurar que o _software_ não causa nenhum vazamento de memória ou ponteiros desnecessários enquanto acessa a memória do sistema. No Rust isso é assegurado por um sistema chamado "_ownership_", com um conjunto de regras que o compilador verifica no momento de compilação.  
O sistema de _ownership_ elimina a necessidade da "coleta de lixo" ou gerenciamento manual de memória, com isso garante uma execução rápida do _software_ e um ambiente de memória mais seguro. As propriedades de gerenciamento de memória do Rust dão suporte para programação concorrente, dando opções para acesso compartilhado e mutável do _state_ que permite mais segurança ao _thread_ e reduzem o risco de insegurança ao _thread_.  
"_Zero-cost abstraction_" é outro conceito chave que o Rust possui. No geral, abstrações em linguagens de programação permitem o código ser escrito em alto nível (como em [Python](https://pt.wikipedia.org/wiki/Python)), sendo capaz de rodar em baixo nível (como em [C](<https://pt.wikipedia.org/wiki/C_(linguagem_de_programa%C3%A7%C3%A3o)>)). Contudo, essas abstrações costumam ser um empecilho no tempo de execução. O Rust possui abstrações, como _iterators_ e _closures_, que não sacrificam performance no tempo de execução. Isso significa que é possível escrever código em alto nível no Rust, e o compilador do Rust otimiza-lo para rodar como se fosse escrito manualmente em código de baixo nível.  
Na maioria dos computadores modernos, manejamento de memória é divido em duas partes principais: o _stack_ (também conhecido como "pilha") e o _heap_ (também conhecido como árvore).

## Sumário

1. [Stack](#stack);
2. [Heap](#heap);
3. [Referência](#referência);
   1. [Referências em artigos da internet](#referências-em-artigos-da-internet);
   2. [Referências em vídeos](#referências-em-vídeos).

## Stack

O _stack_ é uma seção da memória que cresce e encolhe automaticamente assim que a função é chamada e retorna. Para dados serem guardados no _stack_, eles devem ter um tamanho conhecido e fixo na hora de compilar.

## Heap

O _heap_ é uma seção da memória usada para dados que precisam persistir além de uma chamada de função. Dados com tamanho dinâmico são guardados no _heap_.

## Referência

1. [roadmap.sh/rust](https://roadmap.sh/rust).

### Referências em artigos da internet

1. [devmedia.com.br/programacao-com-threads/6152](https://www.devmedia.com.br/programacao-com-threads/6152);
2. [web.mit.edu/rust-lang_v1.25/arch/amd64_ubuntu1404/share/doc/rust/html/book/first-edition/the-stack-and-the-heap.html](https://web.mit.edu/rust-lang_v1.25/arch/amd64_ubuntu1404/share/doc/rust/html/book/first-edition/the-stack-and-the-heap.html).

### Referências em vídeos
