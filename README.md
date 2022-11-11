# Projeto de automação API adotando o framework Cypress com Cucumber

> Esse é um exemplo de como montar uma estrutura inicial de testes automáticos de API com o auxílio do [Cypress.io][cy] e do [cypress-cucumber-preprocessor][cucumber] que dá suporte para a escrita dos cenários com as regras gramaticais do Gherkin e 
com o auxílio do [`cypress-plugin-api`](https://github.com/filiphric/cypress-plugin-api) para visualização das respostas.

## Pre-requirements

It is required to have Node.js and npm installed to run this project.

> I used versions `v16.13.2` and `8.19.2` of Node.js and npm, respectively. I suggest you use the same or later LTS versions.

## Installation

Run `npm install` (or `npm i` for the short version) to install the dev dependencies.

## Tests

> First, you need to create a file called `cypress.env.json`, based on the [`cypress.env.example.json`](./cypress.env.example.json) file.

Run `npm test` (or `npm t` for the short version) to run the test in headless mode.

Or, run `npm run cy:open` to open the Cypress App and run the tests in interactive mode.

## Support this project

If you want to support this project, leave a ⭐.

___

This project was created with 💚 by [Walmyr](https://walmyr.dev).
