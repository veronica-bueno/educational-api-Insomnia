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
**URL Base da API e Swagger:** [Educational - API](https://educational-api-75qy.onrender.com/api-docs/)

**Arquivo Swagger JSON**: [JSON Educational - API](https://educational-api-75qy.onrender.com/swagger.json)

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

* **Usuários:**
    CT001 :: POST - Cadastrar um novo usuário (```/users```)
    CT002 :: POST - Tentativa de cadastro de usuário sem nome (```/users```)
    CT003 :: POST - Tentativa de cadastro de usuário e-mail (```/users```)
    CT004 :: GET - Listar todos os usuários cadastrados (```/users```)
    CT005 :: GET - Tentativa de listar não tendo usuários cadastrados (```/users```)
    CT006 :: GET - Buscando um cadastro de usuário por ID (```/users/id```)
    CT007 :: GET - Tentativa de buscar um usuário não cadastrado por ID não cadastrado (```/users/id```)
    CT008 :: DELETE - Deletando um usuário cadastrado (```/users/id```)
    CT009 :: DELETE - Tentativa de deletar um usuário não cadastrado (```/users/id```)

* **Categorias:**
    CT010 :: POST - Cadastrar uma nova categoria (```/categories```)
    CT011 :: POST - Tentativa de cadastrar nova categoria sem nome (```/categories```)
    CT012 :: POST - Tentativa de cadastrar nova categoria sem descrição (```/categories```)
    CT013 :: GET - Listar todas as categorias cadastradas (```/categories```)
    CT014 :: GET - Buscar categoria por ID (```/categories/id_categories```)
    CT015 :: GET - Tentativa de buscar categoria por ID não cadastrado (```/categories/id_categories```)
    CT016 :: PUT- Atualizando uma categoria cadastrada (```/categories/id_categories```)
    CT017 :: PUT- Tentativa de atualizar uma categoria com ID não cadastrado (```/categories/id_categories```)
    CT018 :: DELETE - Deletando uma categoria (```/categories/id_categories```)
    CT019 :: DELETE - Tentativa de deletar categoria com ID não cadastrado (```/categories/id_categories```)

* **Produtos:**
    CT020 :: POST - Cadastrar um novo produto (```/products```)
    CT021 :: POST - Tentativa de cadastrar novo produto sem nome (```/products```)
    CT022 :: POST - Tentativa de cadastrar novo produto sem a descrição (```/products```)
    CT023 :: GET - Listando todos os produtos cadastrados (```/products```)
    CT024 :: GET - Buscando um produto cadastrado por ID (```/products/id_products```)
    CT025 :: GET - Tentativa de buscar um produto por ID não cadastrado (```/products/id_products```)
    CT026 :: GET - Listar todos os produtos por ID de categoria (```/products/category/id_products```)
    CT027 :: PUT- Atualizando um produto (```/products/id_products```)
    CT028 :: PUT- Tentativa de atualizar um produto com ID inexistente (```/products/id_products```)
    CT029 :: DELETE - Deletando um produto por ID (```/products/id_products```)
    CT030 :: DELETE - Tentativa de deletar um produto com ID inexistente (```/products/id_products```)


* **Pedidos:**
    CT031 :: POST - Cadastrar um novo pedido (```/orders```)
    CT032 :: POST - Tentativa de cadastrar pedido com campos ausentes (```/orders```)
    CT033 :: POST - Tentativa de cadastrar novo pedido com ID não cadastrado (```/orders/id_orders```)
    CT034 :: GET - Listando todos os pedidos cadastrados (```/orders```)
    CT035 :: GET - Buscar pedido cadastrado por ID (```/orders/id_orders```)
    CT036 :: GET - Tentativa de buscar pedido por ID não cadastrado (```/orders/id_orders```)
    CT037 :: GET - Buscando todos os pedidos de um usuário por ID (```/orders/user/id_users```)
    CT038 :: PUT- Atualizar o status de um pedido por ID pedido (```/orders/id_orders/status```)
    CT039 :: PUT - Tentativa de atualizar status do pedido com ID não cadastrado (```/orders/id_orders/status```)
    CT040 :: PUT - Tentativa de atualizar status de pedido com valor inválido (```/orders/id_orders/status```)
    CT041 :: DELETE - Excluindo um pedido por ID (```/orders/id_orders```)
    CT042 :: DELETE - Tentativa de excluir um pedido por ID com ID não cadastrado (```/orders/id_orders```)


📂 **Conteúdo do Repositório**
- Este repositório está organizado para facilitar a visualização da documentação e dos resultados dos testes:

* README.md: Este arquivo, com a descrição geral do projeto.

* ```artefatos/```: Pasta contendo os arquivos de User Story, Plano de Teste, Suíte de Teste e Caso de teste (```.txt```).

* ```evidência/```: Pasta contendo os arquivos de evidências (```.png```) dos testes manuais (screenshots do Insomnia).

    * Organizadas por casos de teste e cenário de teste.

* Para **acesso completo** da execução dos testes manuais, bem como as evidências e documentações, acesse o link do Notion: **URL Projeto API Insomnia:** [Notion Verônica](https://www.notion.so/Testes-Manuais-API-Insomnia-22bf952c68aa80ffbc25f3c56988a9b4)


🚀 **Status do Projeto**
* Finalizado - Todos os testes manuais foram executados e documentados. As evidências foram adicionadas e a pasta ```evidências``` está disponível no repositório dentro de cada endpoint.