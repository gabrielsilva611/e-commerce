# Gs Perfumes - E-commerce de Perfumaria Importada

## Tecnologias Utilizadas

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Node.js, Express
- **Banco de Dados**: MySQL
- **Arquitetura**: MVC (Model-View-Controller)
- **Autenticação**: JWT (JSON Web Token)
- **Testes**: Jest
- **Design**: Figma
- **Versionamento**: Git & GitHub


## Objetivo Geral

Desenvolver uma aplicação web responsiva e segura para o e-commerce GS Perfumes, com foco na venda de perfumes importados, 
oferecendo uma experiência de compra eficiente e intuitiva para os usuários, além de um sistema administrativo completo para gestão de produtos, pedidos e clientes.

## Arquitetura do Sistema

1. Front-end (View)
Desenvolvido com JavaScript

Responsável por toda a interface com o usuário (cliente e administrador)

Consome a API REST do back-end

Aplicação SPA (Single Page Application) com navegação dinâmica

Estilização com CSS

2. Back-end (Controller + Model)
Desenvolvido com Node.js

Responsável pela lógica de negócio e validação de dados

Fornece endpoints REST para o front-end

Implementa autenticação com JWT

3. Banco de Dados (Model)
Sistema Gerenciador: MySQL

Entidades principais: Usuários, Produtos, Pedidos, ItensPedidos, Categorias

Relacionamentos normalizados e com integridade referencial

## Requisitos Funcionais (RF)
RF01, O sistema deve permitir que usuários se cadastrem e realizem login.
RF02, O usuário autenticado pode visualizar e adicionar produtos ao carrinho.
RF03, O sistema deve permitir o cadastro e gerenciamento de produtos (nome, marca, descrição, imagem, preço, estoque).
RF04, O sistema deve permitir a realização de pedidos com escolha de forma de pagamento.
RF05, O sistema deve enviar confirmação por e-mail após o pedido.
RF06, O administrador pode visualizar relatórios de vendas e estoque.
RF07, O sistema deve permitir busca e filtragem de produtos por nome, marca ou categoria.

## Requisitos Não Funcionais (RNF)

RNF01, A interface deve ser responsiva, acessível tanto em dispositivos móveis quanto em desktop.
RNF02, O sistema deve utilizar autenticação segura via JWT.
RNF03, O tempo de resposta do servidor deve ser inferior a 2 segundos para operações comuns.
RNF04, O sistema deve seguir boas práticas de proteção de dados do usuário (LGPD).
RNF05, O banco de dados deve ser hospedado com backup automático diário.

## Justificativa 

Motivos da Escolha:

Separação de responsabilidades: O MVC divide o sistema em camadas distintas — modelo (dados), visão (interface) e controle (lógica), facilitando a organização do código.
Reutilização e manutenção: A modularidade facilita a correção de bugs, adição de novas funcionalidades e testes.
Escalabilidade: A arquitetura pode ser facilmente expandida com novos microserviços ou módulos, conforme a necessidade

## Modelagem

Container: Front-end
Tecnologia: CSS

Funções:

Catálogo de produtos
Página de login/cadastro
Carrinho de compras
Finalização do pedido
Painel administrativo


Container: Back-end (API)
Tecnologia: Node.js + Express

Funções:

Controle de rotas e autenticação (JWT)
Validação de dados e lógica de negócio
Integração com banco de dados
Controle de permissões (usuário vs admin)

Container: Banco de Dados
Tecnologia: MySQL

Tabelas principais:

usuarios (clientes e admins)
produtos
categorias
pedidos
itens_pedido

Relacionamentos: Normalizados com chaves estrangeiras

