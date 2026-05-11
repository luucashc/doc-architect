# Modelos Padrão de Documentação - Time de Engenharia

Este arquivo contém os templates oficiais para documentos no Confluence ou Repositório.

## 1. [PROCESSO] Manual de Operação e Acordos
- **Status:** (Rascunho / Em Vigor / Depreciado)
- **Descrição:** Resumo executivo do processo.
- **Público-alvo:** Quem deve ler este documento.
- **Conteúdo:** Passo a passo ou informações gerais do ritual/acordo.

## 2. [SERVIÇO] Documentação Técnica e de Negócio
- **Status:** (Em Desenvolvimento / Produção / Legado)
- **Contexto de Negócio:** Problema que resolve e regras principais.
- **Arquitetura (C4 Model):** Diagramas Nível 1 e 2, seguidos pela "Visão de Negócio".
- **Dependências:** O que o serviço consome e por quem ele é consumido.
- **Monitoramento:** 
    - **Dashboards:** Links para New Relic, Grafana ou CloudWatch Dashboards.
    - **Logs:** Links para CloudWatch Logs, Kibana ou Splunk.
- **Links Úteis:** GitHub (Repositório), AWS Pipeline CI/CD, Recurso AWS (ECS/Lambda/S3), Swagger.

## 3. [RFC] Estudo de Arquitetura e Decisão
- **Status:** (Em Análise / Aprovado / Rejeitado)
- **Objetivo:** Problema a ser resolvido.
- **Alternativas Consideradas:** Caminhos estudados e motivos do descarte.
- **Solução Proposta:** Diagramas C4, Stack Tecnológica.
- **Estudo de Viabilidade:** Volumetria (QPS), Escalabilidade e Custo (AWS/Cloud).
- **Solicitação:** Link/Status da aprovação no canal de Tech Projects.

## 4. [README] Template Oficial do Repositório (GitHub)
- **Conteúdo:** Contexto de Negócio (1 parágrafo) e Funcionalidades técnicas.
- **Arquitetura:** Princípios (Clean Arch, SOLID, etc).
- **Estrutura de Pastas:** Árvore de diretórios detalhada, expandindo as subpastas da camada de aplicação/núcleo (`app/` ou `src/`) com suas responsabilidades técnicas.
- **Operacional:** Tecnologias/Pré-requisitos, Configuração (.env via .env.example), Comandos de Instalação/Execução e Comandos de Teste.
- **Conectividade:** Links para Confluence, Monitoramento e Squad responsável.


## Elementos Fixos de Cabeçalho
Obrigatório no topo dos modelos 1, 2 e 3.

{indice}

## Status
| Data | Versão | Status |
| :--- | :--- | :--- |
| [DATA_ATUAL] | 1.0 | [RASCUNHO] |
