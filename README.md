# educational-api-Insomnia

### Projeto de Portfólio de Testes de API com Insomnia
- Este repositório apresenta um projeto de portfólio focado em testes de API, demonstrando minhas habilidades em Quality Assurance (QA) através da validação de uma API pública. 
- O projeto envolve a criação de documentação de teste (User Stories e Critérios de Aceitação) e a execução de testes manuais utilizando a ferramenta Insomnia.

🎯 **Objetivo do Projeto**
- O principal objetivo deste projeto é validar o comportamento e a funcionalidade da API pública Educational API, garantindo que os endpoints de Produtos, Usuários, Categorias e Pedidos operem conforme as especificações. 
- Além disso, visa demonstrar minhas competências em:

    - Compreensão e análise de requisitos para API.

    - Criação de User Stories e Critérios de Aceitação claros e concisos.

    - Design de casos de teste para API (cenários de sucesso e falha).

    - Execução de testes manuais de API utilizando uma ferramenta cliente REST (Insomnia).

    - Análise de respostas de API (status codes, corpo JSON, headers).

    - Documentação de resultados de teste e evidências.

🔗 **API Testada**
**URL Base da API e Swagger:** [Educational - API](https://educational-api-production.up.railway.app/api-docs/)

**Arquivo Swagger JSON**: [JSON Educational - API](https://educational-api-production.up.railway.app/swagger.json)

🛠️ **Ferramentas Utilizadas**
- Insomnia

- Swagger/OpenAPI

📝 **Metodologia de Teste** 
- A metodologia de teste aplicada neste projeto segue um fluxo claro:

**Análise de Requisitos:** Compreensão das funcionalidades da API através da documentação Swagger e do entendimento do domínio de negócio.

**Definição de User Stories e Critérios de Aceitação:** Para cada funcionalidade, foram elaboradas User Stories e Critérios de Aceitação detalhados, servindo como base para o design dos testes.

**Design de Casos de Teste:** Com base nos Critérios de Aceitação, foram desenhados cenários de teste abrangendo casos de sucesso, falha (ex: dados inválidos, campos ausentes, IDs inexistentes).

**Execução Manual com Insomnia:** Os casos de teste foram executados manualmente utilizando o Insomnia, enviando requisições HTTP e validando as respostas da API.

**Documentação de Evidências:** Screenshots das requisições e respostas no Insomnia, juntamente com observações, foram coletadas como evidências de teste.

✨ **Funcionalidades Testadas**
Foram criados e executados testes manuais para as seguintes funcionalidades da API:

* **Produtos:**
    - Listagem de todos os produtos (GET ```/products```).
    - Busca de produto por ID (GET ```/products/{id}```).
    - Criação de um novo produto (POST ```/products```).
    - Atualização de um produto existente (PUT ```/products/{id}```).
    - Exclusão de um produto (DELETE ```/products/{id}```).
    - Listagem de produtos por categoria (GET ```/products/category/{categoriaId}```).

* **Usuários:**
    - Cadastro de um novo usuário (POST ```/users```).
    - Listagem de todos os usuários (GET ```/users```).
    - Busca de usuário por ID (GET ```/users/{id}```).
    - Exclusão de um usuário (DELETE ```/users/{id}```).

* **Categorias:**
    - Cadastro de uma nova categoria (POST ```/categories```).
    - Listagem de todas as categorias (GET ```/categories```).
    - Busca de categoria por ID (GET ```/categories/{id}```).
    - Atualização de uma categoria existente (PUT ```/categories/{id}```).
    - Exclusão de uma categoria (DELETE ```/categories/{id}```).

* **Pedidos:**
    - Criação de um novo pedido (POST ```/orders```).
    - Listagem de todos os pedidos (GET ```/orders```).
    - Busca de pedido por ID (GET ```/orders/{id}```).
    - Atualização de status de um pedido (PUT ```/orders/{id}```).
    - Exclusão de um pedido (DELETE ```/orders/{id}```).
    - Listagem de pedidos por usuário (GET ```/orders/user/{userId}```).

📂 **Conteúdo do Repositório**
- Este repositório está organizado para facilitar a visualização da documentação e dos resultados dos testes:

* README.md: Este arquivo, com a descrição geral do projeto.

* ```1. user_story/```: Pasta contendo os arquivos de texto em PDF (```.pdf```) com as User Stories e Critérios de Aceitação para cada funcionalidade.

    * Ex: ```user_story_produtos.pdf```, ```user_story_usuarios.pdf```, etc.

* ```evidência/```: Pasta onde serão armazenadas as evidências dos testes manuais (screenshots do Insomnia).

    * Organizadas por funcionalidade e cenário de teste. Encontra-se dentro de cada respectivo endpoint.


🚀 **Status do Projeto**
* Finalizado - Todos os testes manuais foram executados e documentados. As evidências foram adicionadas e a pasta ```evidências``` está disponível no repositório dentro de cada endpoint.