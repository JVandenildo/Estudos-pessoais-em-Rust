# O sistema Ownership

O conceito de **_ownership_** é uma propriedade importante que governa como o gerenciamento de memória funciona. Cada valor no Rust tem seu próprio "dono" designado, e só pode haver um único dono para um valor por vez. quando o dono sai do escopo, qualquer valor é automaticamente largado da memória. Os três principais pontos do _ownership_ são:

- **Regras do ownership** (**_Ownership rules_**) tem um papel-chave na performance do sistema e prevenção de problemas, como referências vazias ou pendentes;
  1. Cada valor no Rust possui uma variável que é chamada de "_owner_" (dono/dona);
  2. Só pode haver um _owner_ por vez. Isso previne várias partes do código de modificar o dado de uma vez, potencialmente causando inconsistências e corrida de dados;
  3. Quando o _owner_ sai do escopo, o valor é largado. Isso garante que o Rust limpe memória alocada e outros recursos uma vez que não sejam mais necessários, evitando vazamento de memória.
- **Empréstimo** (**_borrowing_**) é um mecanismo onde permitimos algo referenciar um valor sem ter a propriedade (_ownership_) daquilo. Existe dois tipos de empréstimo;
  - Imutável permite vários empréstimos de "somente leitura" de um valor ao mesmo tempo enquanto o valor não mudar; e
  - Mutável permite somente um empréstimo que pode potencialmente modificar o valor.
- **Pedaços** (**_slices_**) são um tipo de dado que não tem um dono. Especificamente, pedaços ajudam a fazer uma referência a uma porção de uma coleção de tipos de dados, como uma `String`, `Array`, ou `Vec`.

## Sumário

1. [Referências](#referências);
   1. [Referências em artigos da internet](#referências-em-artigos-da-internet);
   2. [Referências em vídeos](#referências-em-vídeos).

## Referências

1. [roadmap.sh/rust](https://roadmap.sh/rust).

### Referências em artigos da internet

1. [en.wikipedia.org/wiki/Race_condition](https://en.wikipedia.org/wiki/Race_condition);
2. [rust-book.cs.brown.edu/ch04-01-what-is-ownership.html](https://rust-book.cs.brown.edu/ch04-01-what-is-ownership.html);
3. [rust-book.cs.brown.edu/ch04-02-references-and-borrowing.html](https://rust-book.cs.brown.edu/ch04-02-references-and-borrowing.html);
4. [rust-book.cs.brown.edu/ch04-04-slices.html](https://rust-book.cs.brown.edu/ch04-04-slices.html).

### Referências em vídeos
