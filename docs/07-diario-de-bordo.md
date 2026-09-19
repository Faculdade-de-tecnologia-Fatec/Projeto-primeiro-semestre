# 07 — Diário de bordo

> Registro datado do processo do projeto. **Append-only**: entrada nova vai no
> topo, entrada antiga nunca é editada nem apagada.
>
> Este é o documento que responde às perguntas "como vocês se organizaram?" e
> "qual foi a maior dificuldade?" na apresentação. Ele vale mais na avaliação do
> que parece.

## Como registrar

Uma entrada por marco: reunião, decisão, entrega, obstáculo, material novo no
Drive. Não precisa ser diário de verdade — precisa ser honesto e datado.

```
## AAAA-MM-DD — Título curto

**O que aconteceu:**
**O que mudou no projeto:**
**Decisões:**
**Obstáculos:**
**Próximo passo:**
```

---

## 2026-09-19 — Equipe confirmada e quadro do Trello criado

**O que aconteceu:** Confirmada a composição da equipe pelo quadro do Trello
*PI - 1ºSEMESTRE*: Anderson Rodrigues, Donovan Bueno e João Pedro Sampaio da
Silva. O quadro foi criado com as colunas Levantamento de requisitos,
Levantamento de regras de negócios, Backlog, Desenvolvimento, Testes,
Documentação e Concluído, e tem por enquanto um card de teste.

**O que mudou no projeto:** O trabalho passa a ser tratado como projeto em grupo
de três, o que muda a divisão de tarefas e o roteiro de apresentação
([08-roteiro-de-apresentacao.md](08-roteiro-de-apresentacao.md)).

**Decisões:** Trello como backlog do dia a dia; `docs/` como registro oficial,
com os IDs RF/RN/US aparecendo no título dos cards para amarrar os dois.

**Obstáculos:** O quadro fica na área de trabalho do Donovan e a conta conectada
entrou como convidada, então a leitura automática do quadro não funciona (P-11).
O tema do projeto continua indefinido (P-01).

**Atualização no mesmo dia:** O quadro foi reorganizado por estado — `Backlog`,
`A fazer`, `Fazendo`, `Bloqueado`, `Correção de bug` e `Concluído` — no lugar
das colunas por fase. Fica pendente trocar `Correção de bug` por uma etiqueta
`bug` e nomear as etiquetas (P-10).

**Próximo passo:** Definir o tema e, a partir dele, escrever os primeiros cards
reais com critério de aceite.

## 2026-09-19 — Estrutura de documentação criada

**O que aconteceu:** Montada a estrutura de documentação do projeto no
repositório, junto com o agente de documentação (`.claude/skills/documentador/`)
e a rotina diária de leitura da pasta do Drive.

**O que mudou no projeto:** O projeto passa a ter documentação versionada, em
Markdown, evoluindo por revisões incrementais junto com o código — em vez de um
documento único escrito no fim.

**Decisões:** ADR-01, registrada em
[05-arquitetura-e-tecnologias.md](05-arquitetura-e-tecnologias.md).

**Obstáculos:** Tema do projeto, tecnologia exigida pela disciplina e composição
da equipe ainda não definidos. A pasta do Drive está vazia, então não há material
da disciplina para orientar o escopo.

**Próximo passo:** Subir na pasta do Drive o enunciado da disciplina e a rubrica
de avaliação, e definir o tema. A partir daí, levantar RF, RN e backlog.
