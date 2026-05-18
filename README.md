# doc-architect

O **doc-architect** é um agente especializado em engenharia de documentação técnica. Ele atua de forma proativa na varredura de repositórios para identificar padrões arquiteturais, tecnologias e fluxos de dados, consolidando essas informações em documentos padronizados.

## Contexto de Negócio
Muitas vezes, o conhecimento técnico de um projeto fica isolado na cabeça dos desenvolvedores ou se perde em códigos sem documentação clara. O DocArchitect resolve esse problema automatizando a criação de documentação técnica de alta fidelidade, garantindo que cada repositório possua um README funcional e documentos de serviço prontos para o Confluence, facilitando o onboarding de novos membros e a comunicação com stakeholders.

## Funcionalidades Técnicas
*   **Full Scan de Repositórios:** Varredura automática de diretórios para identificar stack e padrões.
*   **Geração de Diagramas C4:** Criação automática de diagramas de Contexto e Container via Mermaid.
*   **Padronização Corporativa:** Aplicação rigorosa de templates e diretrizes de estilo da engenharia.
*   **Tradução para Negócio:** Resumos analógicos para explicar componentes técnicos a não-técnicos.

## Arquitetura
O projeto segue princípios de **Documentation as Code (DaC)** e **Clean Documentation**, separando as regras de estilo (GEMINI.md) dos modelos estruturais (modelos-padrao-confluence.md).

## Estrutura de Pastas
*   `/`: Raiz do projeto.
    *   `GEMINI.md`: Core de diretrizes e "personalidade" do DocArchitect. Contém as regras inegociáveis de execução.
    *   `diretrizes-confluence.md`: Regras de formatação específicas para garantir compatibilidade com o editor do Confluence.
    *   `modelos-padrao-confluence.md`: Template oficial contendo as seções obrigatórias para README, SERVICO, RFC e PROCESSO.
    *   `README.md`: Documentação principal do repositório (este arquivo).

## Operacional

### Tecnologias e Pré-requisitos
*   Gemini CLI (v1.0.0+)
*   Node.js (para execução do CLI)

### Configuração
As diretrizes de comportamento estão no arquivo `GEMINI.md`. Não há necessidade de variáveis de ambiente específicas além das já configuradas no seu Gemini CLI.

### Comandos
Como este é um agente para Gemini CLI, o uso se dá através do prompt:
```bash
# Para gerar documentação de um projeto
"Gere o README e SERVICO para este projeto seguindo as regras do DocArchitect"
```
