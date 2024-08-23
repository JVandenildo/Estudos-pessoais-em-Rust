# Memory safety e Zero-Cost Abstractions

"_Memory safety_" é assegurar que o _software_ não causa nenhum vazamento de memória ou ponteiros desnecessários enquanto acessa a memória do sistema. No Rust isso é assegurado por um sistema chamado "_ownership_", com um conjunto de regras que o compilador verifica no momento de compilação.  
O sistema de _ownership_ elimina a necessidade da "coleta de lixo" ou gerenciamento manual de memória, com isso garante uma execução rápida do _software_ e um ambiente de memória mais seguro. As propriedades de gerenciamento de memória do Rust dão suporte para programação concorrente, dando opções para acesso compartilhado e mutável do _state_ que permite mais segurança ao _thread_ e reduzem o risco de insegurança ao _thread_.  
"_Zero-cost abstraction_" é outro conceito chave que o Rust possui. No geral, abstrações em linguagens de programação permitem o código ser escrito em alto nível (como em [Python](https://pt.wikipedia.org/wiki/Python)), sendo capaz de rodar em baixo nível (como em [C](<https://pt.wikipedia.org/wiki/C_(linguagem_de_programa%C3%A7%C3%A3o)>)). Contudo, essas abstrações costumam ser um empecilho no tempo de execução. O Rust possui abstrações, como _iterators_ e _closures_, que não sacrificam performance no tempo de execução. Isso significa que é possível escrever código em alto nível no Rust, e o compilador do Rust otimiza-lo para rodar como se fosse escrito manualmente em código de baixo nível.

## Referência

1. [roadmap.sh/rust](https://roadmap.sh/rust).

### Referências em artigos pela _web_

1. [devmedia.com.br/programacao-com-threads/6152](https://www.devmedia.com.br/programacao-com-threads/6152).

### Referências em vídeos
