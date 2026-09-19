# 04 — Backlog do produto

> Última atualização: 2026-09-19
> Convenção de ID: `EP-NN` épico, `US-NNN` user story.

## Épicos

| ID | Épico | Objetivo | US | Status |
|---|---|---|---|---|
| EP-01 | `[A DEFINIR]` | | | Proposto |

## User stories

Formato: **Como** `<ator>`, **quero** `<ação>`, **para** `<benefício>`.
O "para" é obrigatório — se você não consegue escrevê-lo, a história provavelmente
não deveria existir.

| ID | História | Épico | RF | Prioridade | Estimativa | Sprint | Status |
|---|---|---|---|---|---|---|---|
| US-001 | `[A DEFINIR]` | EP-01 | RF-001 | M | — | — | Proposto |

## Detalhamento com critérios de aceite

Uma seção por história, no formato do template
[`templates/template-user-story.md`](templates/template-user-story.md).

### US-001 — `[A DEFINIR]`

> Como `<ator>`, quero `<ação>`, para `<benefício>`.

**Critérios de aceite**

- [ ] **Dado** que … **quando** … **então** …
- [ ] **Dado** que … **quando** … **então** …
- [ ] Caso de erro: **dado** que … **quando** … **então** o sistema exibe a
      mensagem `"…"` e não altera nada.

**Definição de pronto**
- [ ] Funciona nos três tamanhos de tela (360 / 768 / 1280)
- [ ] Sem erro no console
- [ ] Evidência salva em `docs/evidencias/`
- [ ] Documentação atualizada

## Planejamento por sprint

| Sprint | Período | Meta | Histórias | Entregue? |
|---|---|---|---|---|
| 1 | `[A DEFINIR]` | | | — |

## Definição de pronto (geral)

Uma história só é "pronta" quando:

1. O comportamento descrito nos critérios de aceite acontece de verdade no navegador.
2. Não há erro no console.
3. Funciona em 360px, 768px e 1280px.
4. Os campos de formulário têm `label` e mensagem de erro específica.
5. Há evidência (print ou GIF) em `docs/evidencias/`.
6. Os documentos afetados em `docs/` foram atualizados.
7. O código foi commitado com mensagem descritiva.
