# SGCC: Sistema de Gestão Comercial e Catálogo Web

Aplicação web para pequenos empreendedores controlarem vendas, estoque e valores a receber, com um catálogo público integrado ao WhatsApp.

> Este é um repositório de vitrine. O código-fonte pertence à organização do curso (CEUB) e não é público. Aqui descrevo o projeto e a minha participação nele.

## Contexto

- **Instituição:** CEUB, curso de Análise e Desenvolvimento de Sistemas
- **Disciplina:** Projeto Integrador
- **Período:** [02/2026] a [12/2026]
- **Equipe:** 4 pessoas
- **Meu papel:** líder da equipe

## O problema

O cliente do projeto é uma empresa de terraplanagem do Distrito Federal que vende materiais (areia, brita, aterro), presta serviços, aluga máquinas e oferece caminhão pipa. Vendas, estoque e valores a receber eram controlados à mão, em cadernos e planilhas, o que gerava erros, esquecimentos e dificuldade de cobrança. A divulgação era feita mandando fotos e mensagens uma a uma pelo WhatsApp, e os ERPs do mercado eram caros e complexos demais para a realidade da empresa.

## A solução

Uma aplicação web enxuta, em duas frentes integradas:

- **Painel interno:** a equipe controla estoque, vendas, clientes e saldo a receber.
- **Catálogo público:** o cliente final conhece materiais, serviços e máquinas e pede orçamento com um clique pelo WhatsApp.

O objetivo é reduzir a inadimplência, aumentar as vendas e acabar com o controle manual.

## Funcionalidades

- Cadastro de materiais, serviços e locação de máquinas, com unidades próprias da obra (m³, tonelada, viagem, hora, diária)
- Estoque visual com aviso de estoque baixo
- Vendas à vista e a prazo, com local de entrega, vencimento e cancelamento
- Clientes com saldo a receber e cobrança pelo WhatsApp
- Relatórios de vendas por dia, semana e mês
- Catálogo público com pedido de orçamento pelo WhatsApp
- Interface pensada para quem tem pouca familiaridade com sistemas, seguindo as 10 heurísticas de Nielsen

## Minha participação

- **Liderança e gestão ágil:** organizei o backlog e as sprints, dividi as tarefas e revisei pull requests.
- **Backend:** desenvolvi a API em Node.js e Express, a modelagem do banco PostgreSQL e a autenticação com JWT.
- **Frontend:** construí as telas em React, como painel, estoque, vendas, clientes e catálogo público.
- **Integração com WhatsApp:** implementei o pedido de orçamento e a cobrança de clientes pelo WhatsApp.
- **Deploy:** configurei a publicação do frontend, da API e do banco no Render.
- **Documentação:** escrevi [requisitos / decisões de arquitetura / guia de deploy].

Os demais integrantes contribuíram com levantamento de requisitos, testes, parte das telas.

## Stack

| Camada | Tecnologias |
|---|---|
| Frontend | React 18, Vite, React Router |
| Backend | Node.js, Express |
| Banco de dados | PostgreSQL |
| Hospedagem | Render |
| Ferramentas | Git, GitHub, GitHub Projects |

## Arquitetura

O frontend em React consome uma API REST em Node.js e Express, que grava os dados em um banco PostgreSQL. As tabelas são criadas e atualizadas automaticamente quando a API inicia. A autenticação usa tokens JWT, e o acesso à API é restrito ao endereço do site por CORS. Os três componentes são publicados separadamente no Render.

Decisões importantes:

- Fizemos trocas nas tecnologias e plataformas utilizadas por conta de memória, custo e velocidade.  
- O Banco de Dados utilizado estava dando gargalos e ficava indisponível durante algumas horas de pico, trocamos para o nativo do Render.

## Demonstração

- **Sistema no ar:** (https://sgcc-frontend.onrender.com/)

## O que aprendi

- aprendi a usar o git, uso das branches, fazer pull request, uso das issues. 
- levantar requisitos de um cliente.
- publicar e manter uma aplicação
- Uso integrado com IA para código, técnicas de segurança, uso do gitignore.
- Trabalho em equipe, uso de metodologias ágeis como Scrum e Kanban. 

## Contato

- LinkedIn: www.linkedin.com/in/luis-britto-1833bb369
- E-mail: luis.ocbritto@gmail.com
