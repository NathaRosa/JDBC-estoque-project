# 📦 Sistema de Gerenciamento de Estoque de Produtos

Aplicação desktop desenvolvida em Java para gerenciamento de estoque de produtos, com interface gráfica construída utilizando JavaFX e persistência de dados por meio de JDBC.

O projeto foi desenvolvido com o objetivo de praticar conceitos de Programação Orientada a Objetos, manipulação de bancos de dados relacionais e desenvolvimento de interfaces gráficas em Java.

## 🎯 Objetivo do Projeto

Desenvolver uma aplicação que permita gerenciar produtos de maneira simples e organizada, conectando uma interface gráfica Java a um banco de dados relacional.

O projeto explora a integração entre JavaFX, JDBC e SQL, aplicando operações CRUD para manipular os registros de produtos.

## 🚀 Funcionalidades

- **Cadastrar produtos:** adicionar novos produtos ao estoque.
- **Listar produtos:** visualizar os produtos cadastrados em uma tabela.
- **Atualizar produtos:** modificar as informações de um produto selecionado.
- **Excluir produtos:** remover produtos do banco de dados.
- **Selecionar produtos:** preencher os campos do formulário com os dados do produto selecionado.
- **Limpar campos:** redefinir os campos do formulário.
- **Gerenciar informações:** trabalhar com nome, quantidade, preço e status do estoque.

### 📋 Informações dos produtos

Cada produto possui os seguintes atributos:

| Atributo | Descrição |
|---|---|
| ID | Identificador do produto |
| Nome | Nome do produto |
| Quantidade | Quantidade disponível em estoque |
| Preço | Valor unitário do produto |
| Status | Situação do estoque |

O sistema permite selecionar entre os status `Estoque Normal` e `Estoque Baixo`.

## 🛠️ Tecnologias Utilizadas

- **Java:** linguagem utilizada no desenvolvimento da aplicação.
- **JavaFX:** construção da interface gráfica.
- **JDBC (Java Database Connectivity):** comunicação entre a aplicação Java e o banco de dados.
- **SQL:** manipulação e consulta de dados.
- **DAO (Data Access Object):** organização das operações de acesso aos dados.
- **Git e GitHub:** versionamento e disponibilização do código-fonte.

## 🏗️ Organização do Projeto

A aplicação utiliza classes com responsabilidades distintas para organizar a interface gráfica, a representação dos produtos, o acesso aos dados e a conexão com o banco de dados.

| Classe | Responsabilidade |
|---|---|
| `ProdutoGUI` | Construção da interface gráfica e interação com o usuário. |
| `Produto` | Representação dos dados de um produto. |
| `ProdutoDAO` | Execução das operações de acesso e manipulação dos produtos. |
| `ConexaoDB` | Estabelecimento da conexão com o banco de dados. |

Essa separação ajuda a organizar o código e facilita a manutenção e a evolução da aplicação.

## ⚙️ Pré-requisitos

Para executar o projeto, você precisará de:

- JDK compatível com a versão do JavaFX utilizada.
- JavaFX SDK 22.
- Um banco de dados relacional compatível com a implementação JDBC do projeto.
- Driver JDBC correspondente ao banco de dados utilizado.
- IDE Java ou terminal para compilação e execução.

## 📥 Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/NathaRosa/JDBC-estoque-project.git
```

### 2. Acesse o diretório

```bash
cd JDBC-estoque-project
```

### 3. Configure o banco de dados

Configure a conexão com o banco de dados na classe `ConexaoDB`.

Antes de executar a aplicação:

1. Crie ou configure o banco de dados utilizado pelo projeto.
2. Verifique as credenciais e os parâmetros de conexão.
3. Certifique-se de que a estrutura necessária para armazenar os produtos foi criada.
4. Verifique se o driver JDBC correspondente está disponível no classpath.

**Importante:** os parâmetros de conexão e a estrutura do banco devem corresponder à implementação presente no código-fonte.

### 4. Configure o JavaFX

Certifique-se de que o JavaFX SDK esteja instalado e ajuste o caminho para a pasta `lib` de acordo com o ambiente utilizado.

No exemplo abaixo, considera-se que o JavaFX SDK 22 está instalado em:

```text
/usr/lib/jvm/javafx-sdk-22/lib
```

### 5. Compile o projeto

O comando abaixo demonstra a compilação da classe principal:

```bash
javac \
--module-path "/usr/lib/jvm/javafx-sdk-22/lib" \
--add-modules javafx.controls \
ProdutoGUI.java
```

Esse comando pressupõe que as demais classes necessárias estejam acessíveis e que as dependências do projeto estejam configuradas.

Se o projeto utilizar um driver JDBC externo, inclua também o caminho do arquivo JAR correspondente no classpath.

### 6. Execute a aplicação

```bash
java \
--module-path "/usr/lib/jvm/javafx-sdk-22/lib" \
--add-modules javafx.controls \
ProdutoGUI
```

Se houver dependências externas, como um driver JDBC, elas também deverão estar disponíveis durante a execução.

## 📚 Conceitos Praticados

Durante o desenvolvimento deste projeto, são explorados conceitos importantes para a construção de aplicações Java:

- Programação Orientada a Objetos (POO).
- Desenvolvimento de interfaces gráficas com JavaFX.
- Manipulação de eventos.
- Coleções e listas observáveis com `ObservableList`.
- Componentes gráficos, como `TableView`, `TextField`, `ComboBox` e `Button`.
- Conexão com bancos de dados utilizando JDBC.
- Operações CRUD.
- Organização de responsabilidades com o padrão DAO.
- Integração entre interface gráfica e persistência de dados.
- Tratamento de exceções.
- Compilação e execução de aplicações Java pelo terminal.

## 🔮 Possíveis Melhorias Futuras

O projeto pode evoluir com a implementação de funcionalidades adicionais, como:

- Validação dos campos de entrada.
- Tratamento de erros de conexão e de operações no banco de dados.
- Confirmação antes da exclusão de produtos.
- Pesquisa e filtragem de produtos.
- Formatação de preços e valores monetários.
- Indicadores visuais para produtos com estoque baixo.
- Melhorias na organização e no design da interface.
- Testes automatizados.
- Aprimoramento do gerenciamento de conexões com o banco de dados.

## 👨‍💻 Autor

**Natha Rosa**

Estudante de Engenharia de Software, interessado em desenvolvimento de software, Java e construção de aplicações práticas.

Este projeto faz parte da minha jornada de aprendizado, com foco no fortalecimento dos fundamentos da programação e na aplicação prática dos conhecimentos adquiridos.

### 🔗 GitHub

Confira o código-fonte:

[Repositório JDBC Estoque Project](https://github.com/NathaRosa/JDBC-estoque-project)

---

*Projeto desenvolvido para fins de estudo e prática de desenvolvimento de software com Java.*
