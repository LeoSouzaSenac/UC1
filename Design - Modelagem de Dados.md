# Modelagem de Dados

## Diagrama de Entidade-Relacionamento (ER)

### O que é um Diagrama ER?

Um Diagrama de Entidade-Relacionamento (ER) é uma representação visual de como os dados em um sistema estão organizados e como se relacionam entre si. Ele funciona como um mapa, permitindo que você entenda a estrutura e as conexões dos dados.

### Componentes de um Diagrama ER:

- **Entidades**: São as "coisas" ou "objetos" principais sobre os quais queremos armazenar informações. Exemplo: Livros, Clientes, Vendas.
- **Atributos**: São as informações que descrevem as entidades. Exemplo: Para a entidade Livros, os atributos podem ser Título, Autor, Preço, Quantidade em Estoque.
- **Relacionamentos**: Mostram como as entidades estão conectadas. Exemplo: Um relacionamento pode mostrar que "um cliente pode comprar muitos livros" e "um livro pode ser comprado por muitos clientes".

### Por que usar um Diagrama ER?

- **Clareza**: Ajuda a visualizar e entender a organização dos dados.
- **Planejamento**: Facilita o planejamento de como os dados serão armazenados em um banco de dados.
- **Comunicação**: Serve como uma ferramenta para comunicar a estrutura dos dados com outras pessoas envolvidas no projeto, como desenvolvedores e clientes.

### Exemplo Prático:

- **Entidades**: 
  - Livros (Título, Autor, Preço, Quantidade)
  - Clientes (Nome, Contato)
  - Vendas (Data da Venda, Livro Vendido, Cliente)

- **Relacionamentos**: 
  - Um Cliente pode fazer muitas Vendas.
  - Uma Venda pode incluir muitos Livros.

Esse diagrama ajudará a entender como os dados relacionados a livros, clientes e vendas estão organizados e conectados no sistema.
