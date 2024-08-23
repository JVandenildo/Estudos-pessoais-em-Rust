# O sistema Ownership

O conceito de **_ownership_** é uma propriedade importante que governa como o gerenciamento de memória funciona. Cada valor no Rust tem seu próprio "dono" designado, e só pode haver um único dono para um valor por vez. quando o dono sai do escopo, qualquer valor é automaticamente largado da memória. Os três principais pontos do _ownership_ são:

- **Regras do ownership** (**_Ownership rules_**) tem um papel-chave na performance do sistema e prevenção de problemas, como referências vazias ou pendentes;
- **Empréstimo** (**_borrowing_**) é um mecanismo onde permitimos algo referenciar um valor sem ter a propriedade (_ownership_) daquilo;
- **Pedaços** (**_slices_**) são um tipo de dado que não tem um dono. Especificamente, pedaços ajudam a fazer uma referência a uma porção de uma coleção de tipos de dados, como uma `String`, `Array`, ou `Vec`.

## Sumário

1. [Referências](#referências);
   1. [Referências em artigos da internet](#referências-em-artigos-da-internet);
   2. [Referências em vídeos](#referências-em-vídeos).

## Referências

1. [roadmap.sh/rust](https://roadmap.sh/rust).

### Referências em artigos da internet

### Referências em vídeos
