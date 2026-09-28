$readmeContent = @"
# Agenda de Contatos

Projeto didático desenvolvido em Java para acompanhar a evolução dos conceitos trabalhados na disciplina de Programação Orientada a Objetos.

O sistema é desenvolvido de forma incremental. Cada versão introduz novos conceitos, estruturas e melhorias sobre a versão anterior.

## Objetivo

Construir uma Agenda de Contatos completa, iniciando com uma solução procedural simples e evoluindo gradualmente para uma aplicação organizada com conceitos de Programação Orientada a Objetos, interface gráfica e persistência de dados.

## Evolução do projeto

| Versão | Armazenamento | Descrição |
|---|---|---|
| v0.0.0 | Variáveis simples | Permite armazenar apenas um contato |
| v0.1.0 | Arrays | Permite vários contatos com capacidade fixa |
| v0.2.0 | List + ArrayList | Permite vários contatos com tamanho dinâmico |
| v0.3.0 | List + ArrayList | Adiciona a opção de alteração de contatos cadastrados |
| v1.0.0 | List + ArrayList | Modularização das funcionalidades com métodos |
| v1.1.0 | List + ArrayList | Separação em múltiplos arquivos (Uteis e Agenda) |
| v1.1.1 | List + ArrayList | Correção de bug na opção SAIR |
| v2.1.0 | Arquivo de Texto (`contato.txt`) | Persistência de dados com classe `Persistencia` |

### v0.0.0 — Programação Procedural Básica

Primeira versão da Agenda.

Principais características:

- uma única classe ``Principal``;
- todo o código dentro do método ``main()``;
- armazenamento de apenas um contato;
- variáveis ``nome``, ``celular`` e ``email``;
- menu em console;
- uso de ``Scanner``;
- uso de ``if-else``;
- uso de ``switch-case``;
- uso de ``while``;
- funcionalidades:
  - adicionar contato;
  - listar contato;
  - procurar contato;
  - excluir contato;
  - sair.

Nesta versão, um novo contato substitui o contato armazenado anteriormente.

### v0.1.0 — Arrays e Capacidade Fixa

Segunda versão da Agenda.

Principais características:

- uso de arrays simples (``String[]``) para cada atributo;
- controle de capacidade máxima pré-definida;
- manipulação através de índices e estrutura ``for``;
- busca sequencial nos arrays;
- remoção de elementos com reorganização física do array (deslocamento de itens).

### v0.2.0 — Armazenamento Dinâmico com ArrayList

Terceira versão da Agenda.

Principais características:

- uso da API de Coleções do Java (``List`` e ``ArrayList``);
- uso de Generics (````);
- alocação e redimensionamento dinâmico;
- métodos da API (``add``, ``get``, ``remove``, ``size``, ``indexOf``, etc.);
- iteração com ``for-each``;
- simplificação das operações de inserção, busca e remoção.

### v0.3.0

Nesta versão, a Agenda de Contatos recebeu a implementação da funcionalidade de **alteração de contatos**.

### Principais características e conceitos

- Nova opção no menu: **Alterar contato**
- Busca do contato a ser alterado
- Atualização dos dados nas listas (``List`` / ``ArrayList``) utilizando o método ``set()``
- Reutilização da lógica de validação/busca para localização do registro antes da modificação

## V1.0.0 - Modularização das funcionalidades

Nesta versão, o projeto Agenda de Contatos foi reorganizado por meio da criação de métodos.

### Principais alterações

- Modularização do código procedural.
- Criação dos métodos `adicionar()`, `listar()`, `pesquisar()`, `atualizar()` e `excluir()`.
- Simplificação do ``switch-case``.
- Uso de parâmetros para compartilhar os dados entre os métodos.

## V1.1.0 e V1.1.1 - Organização e Correções

- **V.1.1.0**: Modularização das funcionalidades em arquivos separados (Uteis e Agenda).
- **V.1.1.1**: Ajustes de estabilidade e correção de bug no encerramento (opção SAIR).

## V2.1.0 - Persistência de Dados em Arquivo de Texto

Nesta versão, o projeto passa a salvar os contatos de forma permanente em disco, garantindo que os dados não sejam perdidos ao fechar a aplicação.

### Principais alterações e conceitos

- Criação da classe **Persistencia** para gerenciar a leitura e escrita de arquivos.
- Uso do arquivo **`contato.txt`** para armazenamento físico dos contatos.
- Leitura automática dos dados salvos no início da aplicação.
- Atualização e gravação automática do arquivo ao inserir, editar ou remover contatos.

## Controle de versões

As versões estáveis do projeto são identificadas por tags Git.

Exemplo:

```text
- V0
  - V0.0.0
  - V0.1.0
  - V0.2.0
  - V0.3.0
- V1
  - V1.0.0
  - V1.1.0
  - V1.1.1
- V2
  - V2.1.0
