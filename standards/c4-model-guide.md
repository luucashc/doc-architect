# Guia de C4 Model e Diagramas (Mermaid.js)

## 1. Regras de Sintaxe do Mermaid (Skin C4 Oficial)
Utilize obrigatoriamente a biblioteca nativa C4 do Mermaid, evitando fluxogramas genéricos (`graph TD` ou `graph LR`).

* Nível 1 (Contexto): Inicie o bloco com `C4Context`
* Nível 2 (Container): Inicie o bloco com `C4Container`

### Elementos Permitidos:
* `Person(alias, "Nome", "Descrição")`
* `System(alias, "Nome", "Descrição")`
* `System_Boundary(alias, "Nome") { ... }`
* `Container(alias, "Nome", "Tecnologia", "Descrição")`
* `ContainerDb(alias, "Nome", "Tecnologia", "Descrição")`
* `ContainerQueue(alias, "Nome", "Tecnologia", "Descrição")`
* `Rel(origem, destino, "Ação", "Tecnologia/Protocolo")`

## 2. Estrutura de Entrega
Sempre que gerar este diagrama, a sua resposta deve conter:
1.  **O Diagrama:** Bloco de código ```mermaid.
2.  **Em resumo (Visão Técnica):** Bullet points sobre o fluxo de dados e Tech Stack.
3.  **Em resumo (Visão de Negócio):** Texto simples e analógico para stakeholders, focado em valor e objetivo, sem jargões de infraestrutura.