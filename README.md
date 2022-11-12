# Projeto de automação API adotando o framework Cypress com Cucumber

> Esse é um exemplo de como montar uma estrutura inicial de testes automáticos de API com o auxílio do [`Cypress.io`](https://github.com/cypress-io/cypress) e do [`cypress-cucumber-preprocessor`](https://github.com/badeball/cypress-cucumber-preprocessor) que dá suporte para a escrita dos cenários com as regras gramaticais do Gherkin e 
com o auxílio do [`cypress-plugin-api`](https://github.com/filiphric/cypress-plugin-api) para visualização das respostas.

![Vídeo-sem-título](https://user-images.githubusercontent.com/19351435/201253753-74a78656-919a-469f-a516-334afe77756f.gif)


### ✨ Pré-requisitos
-----------------------
- A IDE escolhida foi o [`VS Code`](https://code.visualstudio.com/download);
- Instale o [`Node.js`](https://nodejs.org/en/download/);
- Seguindo as instruções da documentação do [`Cypress.io`](https://github.com/cypress-io/cypress), do [`cypress-cucumber-preprocessor`](https://github.com/badeball/cypress-cucumber-preprocessor) e do [`cypress-plugin-api`](https://github.com/filiphric/cypress-plugin-api) os instale;
- Baixe este repositório ou faça um git clone;
- Abra o diretório do projeto e execute o comando:
    - `npm install`
- Para acionar os testes, execute no diretório do projeto:
    - `npm run run`
- Pronto, o projeto será executado em sua máquina.😄

### ⚙️ Arquitetura do projeto
-----------------------

```
  ├─  cypress/
  │        │
  │        ├── e2e/
  │        │   ├── assertions
  │        │       └── assertions.js
  │        │   ├── features
  │        │       └── get.features
  │        │   ├── requests
  │        │       └── requests.js
  │        │   ├── step_definitions
  │        │       └── get.spec.js
  │        ├── support/
  │        │   └── commands.js
  │        │   └── e2e.js
  ├── cypress.config.json
  ├── package.json
  └── README.md
```
---------------------------------------
## 🔍 Camadas da arquitetura

 - **assertions:** estratégia para executar as assertivas dos parametros retornados pela requisição;
 - **features:** arquivos contendo as definições de BDD em extensão *.feature;
 - **requests:** estratégia apra realização de requisições;
 - **step_definitions:** contém a junção entre a definição do BDD as chamdas dos requests e assertions para efetivação da validação
