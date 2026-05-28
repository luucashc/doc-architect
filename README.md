# doc-architect

## Contexto de Negócio
Agente especializado em engenharia de documentação técnica, projetado para realizar varreduras em repositórios e gerar proativamente artefatos padronizados. O projeto resolve o problema da fragmentação de conhecimento e falta de padrão em documentações de sistemas, automatizando a criação de READMEs, manuais de serviço e registros de processos seguindo as melhores práticas de engenharia.

## Funcionalidades técnicas
* Geração automatizada de documentação técnica (README, SERVICO, PROCESSO).
* Padronização de diagramas de arquitetura utilizando C4 Model via Mermaid.js.
* Validação de conformidade com diretrizes organizacionais e guias de estilo.
* Mapeamento de estruturas de pastas com análise de responsabilidades por camada.
* Suporte a múltiplos templates e contextos de negócio dinâmicos.

## Arquitetura
O projeto fundamenta-se nos princípios de **Documentation as Code** e **Standardization First**, operando sob as seguintes camadas:

* **Camada Comportamental:** Lógica de decisão e tom de voz centralizados em arquivos de diretrizes (`GEMINI.md`).
* **Camada Normativa:** Definição de padrões técnicos e sintaxe obrigatória para diagramas e fluxos.
* **Camada Estrutural:** Templates modulares que garantem a consistência visual e organizacional entre diferentes tipos de documentos.

## Estrutura de Pastas
A organização do repositório segue uma lógica de separação entre diretrizes de execução, normas técnicas e modelos de saída:

* `GEMINI.md`: Arquivo mestre de diretrizes. Contém as instruções inegociáveis de comportamento, formatação e fluxo de resposta do agente.
* `docs/`: Documentação de suporte ao usuário e manuais operacionais.
    * `how-to-use.md`: Guia prático detalhando comandos, exemplos de interação e melhores práticas de uso do agente.
* `standards/`: Camada normativa contendo as regras de negócio técnicas.
    * `c4-model-guide.md`: Define a sintaxe obrigatória para diagramas de arquitetura, garantindo conformidade com o padrão C4.
* `templates/`: Repositório de modelos estruturais que servem de base para a geração de novos artefatos.
    * `confluence-documentation.md`: Esqueletos oficiais para documentos do tipo `[PROCESSO]`, `[SERVIÇO]` e `[README]`.

## Operacional

### Tecnologias/Pré-requisitos
* Gemini CLI (Interface de execução e orquestração do agente)
* Markdown (Linguagem de marcação para os documentos técnicos)
* Mermaid.js (Motor para renderização de diagramas e fluxogramas)

### Configuração
Este projeto não utiliza variáveis de ambiente ou arquivos `.env`. Todas as diretrizes operacionais e configurações de contexto estão centralizadas no arquivo `GEMINI.md`.

Para detalhes sobre como interagir com o agente e exemplos de comandos, consulte o guia prático em: [how-to-use.md](docs/how-to-use.md).

## Conectividade
* **GitHub:** [Repositório Oficial](https://github.com/luucashc/doc-architect)
