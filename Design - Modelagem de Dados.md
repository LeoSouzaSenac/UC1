# Modelagem de Dados

## Diagrama de Entidade-Relacionamento (ER)

### O que é um Diagrama ER?

Um Diagrama de Entidade-Relacionamento (ER) é uma representação visual de como os dados em um sistema estão organizados e como se relacionam entre si. Ele funciona como um mapa, permitindo que você entenda a estrutura e as conexões dos dados.

### Componentes de um Diagrama ER:

- **Entidades**: São as "coisas" ou "objetos" principais sobre os quais queremos armazenar informações. Exemplo: Livros, Clientes, Vendas. Elas são representadas por retângulos.
- **Atributos**: São as informações que descrevem as entidades. Exemplo: Para a entidade Livros, os atributos podem ser Título, Autor, Preço, Quantidade em Estoque. Os atributos são representados por círculos com seu nome e são conectados à entidade com uma linha.
- **Relacionamentos**: Mostram como as entidades estão conectadas. Exemplo: Um relacionamento pode mostrar que "um cliente pode comprar livros" e "um livro pode ser comprado pelos clientes". Relacionamentos são representados por losangos e são conectados às entidades envolvidas com linhas.

### Cardinalidade

A **cardinalidade** descreve a quantidade de instâncias de uma entidade que podem se associar a uma instância de outra entidade. Em um Diagrama ER, a cardinalidade ajuda a definir a natureza dos relacionamentos entre entidades. Existem três tipos principais de cardinalidade:

1. **Um-para-Um (1:1)**:
   - **Definição**: Cada instância de uma entidade está associada a no máximo uma instância de outra entidade e vice-versa.
   - **Exemplo**: Um **"Número de Identidade"** pode estar associado a apenas uma **"Pessoa"**, e uma **"Pessoa"** pode ter apenas um **"Número de Identidade"**.
   - **Representação**: Linha conectando duas entidades com a anotação `1` em ambas as extremidades.

2. **Um-para-Muitos (1:N)**:
   - **Definição**: Uma instância de uma entidade pode estar associada a várias instâncias de outra entidade, mas cada instância da segunda entidade está associada a no máximo uma instância da primeira entidade.
   - **Exemplo**: Um **"Departamento"** pode ter vários **"Funcionários"**, mas cada **"Funcionário"** pertence a apenas um **"Departamento"**.
   - **Representação**: Linha conectando duas entidades com a anotação `1` em um lado e `N` no outro.

3. **Muitos-para-Muitos (M:N)**:
   - **Definição**: Uma instância de uma entidade pode estar associada a várias instâncias de outra entidade, e vice-versa.
   - **Exemplo**: Um **"Aluno"** pode se matricular em vários **"Cursos"**, e um **"Curso"** pode ter vários **"Alunos"** matriculados.
   - **Representação**: Linha conectando duas entidades com a anotação `M` em ambos os lados.

### Por que usar um Diagrama ER?

- **Clareza**: Ajuda a visualizar e entender a organização dos dados.
- **Planejamento**: Facilita o planejamento de como os dados serão armazenados em um banco de dados.
- **Comunicação**: Serve como uma ferramenta para comunicar a estrutura dos dados com outras pessoas envolvidas no projeto, como desenvolvedores e clientes.

## Exemplo Prático:

### Entidades:

- **Farmácia**
  - **Atributos**:
    - Telefone
    - Nome
    - Endereço
    - CNPJ

- **Produto**
  - **Atributos**:
    - Código
    - Quantidade
    - Valor

- **Farmacêutico**
  - **Atributos**:
    - RG
    - Nome

### Relacionamentos:

- **Vende**
  - **Descrição**: O relacionamento "Vende" conecta a entidade **Farmácia** com a entidade **Produto**. Ele indica que uma farmácia pode vender vários produtos e um produto pode ser vendido por várias farmácias.
  - **Cardinalidade**: Muitos-para-Muitos (M:N)
    - Uma farmácia pode vender muitos produtos.
    - Um produto pode ser vendido por muitas farmácias.

- **Atendimento**
  - **Descrição**: O relacionamento "Atendimento" conecta a entidade **Farmacêutico** com a entidade **Farmácia**. Ele indica que um farmacêutico pode trabalhar em várias farmácias e uma farmácia pode ter vários farmacêuticos.
  - **Cardinalidade**: Muitos-para-Muitos (M:N)
    - Um farmacêutico pode trabalhar em muitas farmácias.
    - Uma farmácia pode ter muitos farmacêuticos.

Neste diagrama, as cardinalidades ajudam a definir quantos clientes podem fazer vendas e quantos livros podem estar associados a uma venda. O diagrama ajuda a entender como os dados relacionados a livros, clientes e vendas estão organizados e conectados no sistema.
