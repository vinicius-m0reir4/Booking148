Booking API Testing — Playwright

Projeto de testes automatizados de API desenvolvido com **Playwright e JavaScript**, utilizando a API pública [Restful Booker](https://restful-booker.herokuapp.com/).

O objetivo é validar as principais operações de gerenciamento de reservas, aplicando conceitos de testes funcionais de API, validação de respostas HTTP, autenticação e operações CRUD.

## Tecnologias utilizadas

- **JavaScript** — linguagem dos testes.
- **Playwright** — execução e validação dos testes de API.
- **Node.js e npm** — ambiente de execução e gerenciamento de dependências.
- **Git e GitHub** — versionamento e publicação do projeto.

## Cenários de teste

| Cenário | Método HTTP | Objetivo |
|---|---|---|
| Autenticação | POST | Validar o login e a geração do token |
| Criar reserva | POST | Criar uma reserva e validar os dados retornados |
| Consultar reserva | GET | Consultar uma reserva pelo ID |
| Atualizar reserva | PUT | Validar a atualização completa dos dados |
| Atualizar parcialmente | PATCH | Validar a alteração de campos específicos |
| Excluir reserva | DELETE | Validar a exclusão da reserva |

## Conceitos aplicados

- Validação de status codes HTTP.
- Verificação do conteúdo das respostas JSON.
- Uso de assertions com `expect`.
- Captura e reutilização dinâmica do ID da reserva.
- Autenticação por token para operações protegidas.
- Organização de testes com `test.describe.serial`.
- Estruturação dos testes em Arrange, Act e Assert.

## Como executar o projeto

### Pré-requisitos

- Node.js instalado.
- Git instalado.
- Acesso à internet para consultar a API.

### 1. Clonar o repositório

```bash
git clone https://github.com/vinicius-m0reir4/Booking148.git
```

### 2. Acessar a pasta

```bash
cd Booking148
```

### 3. Instalar as dependências

```bash
npm install
```

### 4. Executar os testes

```bash
npx playwright test
```

Para executar os testes com saída detalhada:

```bash
npx playwright test --reporter=list
```

## API utilizada

**Restful Booker**

Base URL: https://restful-booker.herokuapp.com

Documentação: https://restful-booker.herokuapp.com/apidoc/index.html

A API é utilizada para praticar operações de autenticação e gerenciamento de reservas.

## Observações

- A API utilizada é pública e destinada à prática de testes.
- A disponibilidade e os dados da API podem variar.
- Os testes utilizam uma sequência de execução para compartilhar o ID da reserva e o token de autenticação.
- O projeto tem finalidade educacional e de desenvolvimento de habilidades em QA.

## Autor

**Vinicius Moreira**

Estudante de Sistemas de Informação, com foco em Qualidade de Software (QA), testes de API e automação de testes.
