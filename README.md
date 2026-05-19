# doc-architect

Agente especializado em engenharia de documentação técnica, projetado para atuar na varredura de repositórios e geração proativa de documentação padronizada para times de engenharia.

## Descrição do Projeto

O **doc-architect** automatiza a criação de artefatos essenciais como READMEs, manuais de serviço e definições de processo. O projeto utiliza engenharia de prompt avançada para garantir que a documentação técnica seja consistente, impessoal e tecnicamente precisa, facilitando a manutenção do conhecimento e o onboarding de novos desenvolvedores.

## Arquitetura

O projeto baseia-se nos princípios de **Documentation-as-Code** e **Standardization First**. A lógica de operação é desacoplada em três camadas principais:
*   **Comportamental:** Regras de negócio e tom de voz definidos no core do agente.
*   **Normativa:** Guias de sintaxe (como C4 Model) que garantem a qualidade técnica dos diagramas.
*   **Estrutural:** Templates pré-definidos que asseguram a consistência visual e organizacional entre diferentes projetos.

## Estrutura de Pastas

A organização do repositório segue uma lógica de separação entre diretrizes de execução e modelos de saída:

*   `GEMINI.md`: Arquivo central de diretrizes. Contém as instruções inegociáveis de comportamento, formatação e fluxo de resposta do agente.
*   `standards/`: Camada normativa do projeto.
    *   `c4-model-guide.md`: Define a sintaxe obrigatória para diagramas de arquitetura, utilizando a biblioteca nativa C4 do Mermaid.js.
*   `templates/`: Repositório de modelos estruturais.
    *   `confluence-documentation.md`: Contém os esqueletos oficiais para os documentos do tipo `[PROCESSO]`, `[SERVIÇO]` e `[README]`.

## Operacional

### Tecnologias e Pré-requisitos
*   Gemini CLI (Interface de execução do agente)
*   Markdown (Linguagem de marcação para os documentos)
*   Mermaid.js (Motor de renderização de diagramas)

### Configuração
O agente não requer variáveis de ambiente locais. Sua configuração é integralmente baseada no arquivo `GEMINI.md`. Certifique-se de que o contexto do repositório está carregado no Gemini CLI antes de iniciar as solicitações.

### Comandos de Exemplo
Para interagir com o agente, utilize comandos naturais via CLI:
*   `"Gere um [README] para este projeto."`
*   `"Crie a documentação de [SERVIÇO] seguindo o template oficial."`
*   `"Mapeie o fluxo deste repositório e gere um [PROCESSO]."`

## Conectividade e Recursos

*   **Repositório:** [GitHub - doc-architect](https://github.com/exemplo/doc-architect)
*   **Documentação:** [Confluence - Engineering Hub](https://confluence.exemplo.com/display/ENG/DocArchitect)
*   **Monitoramento:** Logs de execução via console do Gemini CLI.
