# doc-architect

Agente especializado em engenharia de documentação técnica, projetado para atuar na varredura de repositórios e geração proativa de documentação técnica padronizada.

## Descrição do Projeto
O **doc-architect** automatiza a criação de documentos como README, manuais de serviço e definições de processo. Utilizando varreduras profundas, o agente identifica padrões arquiteturais e tecnológicos, consolidando-os em artefatos prontos para publicação em plataformas como Confluence.

## Tecnologias e Pré-requisitos
*   Gemini CLI
*   Markdown

## Estrutura de Pastas

### Camadas de Configuração e Padrões
*   `GEMINI.md`: Core de diretrizes, regras de execução e comportamento do agente DocArchitect. Define o fluxo de trabalho e restrições de saída.
*   `standards/`: Diretório contendo normas técnicas e guias de modelagem.
    *   `c4-model-guide.md`: Guia de referência para a criação de diagramas seguindo a metodologia C4 Model (Contexto, Container, Componente e Código).
*   `templates/`: Repositório de modelos estruturais para documentos.
    *   `confluence-documentation.md`: Modelo padronizado para documentação de serviços, otimizado para o editor do Confluence.

## Configuração
O comportamento do agente é regido pelas instruções contidas no arquivo `GEMINI.md`. Para utilizar o DocArchitect, certifique-se de que o Gemini CLI está configurado e que este repositório está acessível como contexto de execução.

## Operacional

### Fluxo de Trabalho
1.  **Scan:** Diagnóstico da stack e arquitetura.
2.  **Geração:** Criação de arquivos `.md` na raiz do projeto conforme a necessidade (`README.md`, `SERVICO.md` ou `PROCESSO.md`).

### Comandos de Exemplo
```bash
"Gere um [README] para este projeto."
"Crie o documento de [SERVIÇO] com diagramas Mermaid."
```

## Conectividade e Recursos
*   **Repositório:** GitHub (Origem dos fontes e padrões)
*   **Documentação Corporativa:** Confluence (Destino final dos documentos de serviço)

## Observabilidade e Logs
A observabilidade do agente é realizada através dos logs de execução do Gemini CLI, que reportam o status de geração e mapeamento de seções de cada documento processado.
