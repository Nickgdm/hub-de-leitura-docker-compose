╔══════════════════════════════════════════════════════╗
║          HUB DE LEITURA — AMBIENTE DOCKER COMPOSE     ║
╚══════════════════════════════════════════════════════╝

Projeto de estudo que integra a aplicação Hub de Leitura com uma suíte de testes de interface, utilizando Docker Compose para organizar o ambiente de execução.

══════════════════════════════════════════════════════

## Sobre o projeto

O repositório descreve serviços da aplicação e dos testes de UI, além de volumes destinados a armazenar logs e artefatos de execução.

══════════════════════════════════════════════════════

## Objetivos

- Definir serviços e dependências por meio do Docker Compose.
- Preparar a aplicação e os testes de UI para execução em ambiente integrado.
- Organizar logs e artefatos de execução.

══════════════════════════════════════════════════════

## Tecnologias e ferramentas

- Docker
- Docker Compose
- Hub de Leitura
- Cypress para automação de UI, conforme o projeto de testes integrado

══════════════════════════════════════════════════════

## Pré-requisitos

- Docker Engine e Docker Compose instalados.
- Git instalado.
- Portas exigidas pelos serviços livres no computador.

══════════════════════════════════════════════════════

## Como executar

1. Clone o repositório e entre no diretório.
2. Revise os serviços, as portas, os volumes e as variáveis em `docker-compose.yml`.
3. Inicie o ambiente:

```bash
docker compose up --build
```

4. O serviço `teste-ui` está configurado com `command: npm test`. Acompanhe os logs para verificar a execução e o resultado dos testes.
5. Para encerrar o ambiente:

```bash
docker compose down
```

Os vídeos e as capturas de tela são mapeados para a pasta local `logs/`, conforme os volumes configurados no Compose.

══════════════════════════════════════════════════════

## Estrutura do projeto

```text
atividade-docker-hub-de-leitura/
├── docker-compose.yml
├── hub-de-leitura-integrado/
├── hub-de-leitura-teste-ui/
├── logs/
└── README.md
```

══════════════════════════════════════════════════════

## Desafios práticos

- Integrar a aplicação e a suíte de testes.
- Configurar a comunicação entre containers.
- Diagnosticar problemas utilizando os logs.

══════════════════════════════════════════════════════

## Boas práticas

- Descrever o ambiente como código.
- Separar a aplicação integrada dos testes de UI.
- Manter um diretório dedicado aos logs.
- Conferir a inicialização dos serviços antes de interpretar os resultados dos testes.

══════════════════════════════════════════════════════

## Aprendizados

A atividade permite praticar o uso do Docker Compose para coordenar serviços e preparar um ambiente integrado para automação. Também reforça a importância de conferir a inicialização da aplicação e consultar logs ao investigar falhas.

══════════════════════════════════════════════════════

## Considerações finais

A aplicação e os testes são definidos como serviços em `docker-compose.yml`. Revise as configurações e consulte os logs para confirmar a inicialização da aplicação e o resultado da suíte.

══════════════════════════════════════════════════════

## Formação e natureza da atividade

Este projeto foi desenvolvido como uma **atividade facultativa** no contexto dos estudos de Quality Assurance (QA), durante a formação da EBAC — Escola Britânica de Artes Criativas e Tecnologia. Seu objetivo é praticar e consolidar conhecimentos de Docker Compose e automação de testes.

══════════════════════════════════════════════════════