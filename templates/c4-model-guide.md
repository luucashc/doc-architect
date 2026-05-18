# Guia de C4 Model e Diagramas (Mermaid.js)

## 1. Regras de Sintaxe do Mermaid (Skin C4 Oficial)
Você NUNCA deve usar fluxogramas genéricos (`graph TD` ou `graph LR`). 
Você DEVE obrigatoriamente usar a biblioteca nativa de C4 do Mermaid.

* Para Nível 1, inicie o bloco com: `C4Context`
* Para Nível 2, inicie o bloco com: `C4Container`

### Elementos Permitidos:
* `Person(alias, "Nome", "Descrição")`
* `System(alias, "Nome", "Descrição")`
* `System_Boundary(alias, "Nome") { ... }`
* `Container(alias, "Nome", "Tecnologia", "Descrição")`
* `ContainerDb(alias, "Nome", "Tecnologia", "Descrição")`
* `ContainerQueue(alias, "Nome", "Tecnologia", "Descrição")`
* `Rel(origem, destino, "Ação", "Tecnologia/Protocolo")`

## 2. Estrutura de Entrega (Obrigatório)
Sempre que gerar um diagrama, a sua resposta deve seguir exatamente esta estrutura visual:

1.  **O Diagrama:** O bloco de código ```mermaid gerado com as regras acima.
2.  **Em resumo (Visão Técnica):** Um parágrafo rápido (bullet points) sobre o fluxo de dados e os serviços AWS/Tech Stack utilizados.
3.  **Em resumo (Visão de Negócio):** Um parágrafo explicando o fluxo de forma simples, analógica e focada em valor, voltada para stakeholders não-técnicos (Product Managers, Diretores). Explique *o que* o sistema resolve e *por que* isso é seguro/rápido/barato, sem usar jargões de infraestrutura.