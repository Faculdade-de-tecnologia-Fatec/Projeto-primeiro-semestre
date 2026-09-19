# 06 — Padrões de código

> Última atualização: 2026-09-19
> Estes padrões existem para que o código de todos os integrantes pareça escrito
> pela mesma pessoa. A banca percebe quando não parece.

## HTML

- Sempre semântico: `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`.
  `div` só quando não houver elemento semântico que sirva.
- `lang="pt-BR"` no `<html>` e `<meta charset="UTF-8">`.
- Todo `<img>` com `alt` descritivo. Imagem decorativa: `alt=""`.
- Todo `<input>` com `<label for="...">`. Placeholder **não** substitui label.
- Botão que executa ação é `<button>`, não `<div onclick>`.
- Indentação de 2 espaços.

## CSS

- Variáveis em `:root` para cor, fonte e espaçamento. Nada de hex solto no meio
  do arquivo.
- Nomes de classe em `kebab-case`, descrevendo função e não aparência:
  `.card-agendamento`, não `.caixa-azul`.
- Mobile first: escreva o estilo base para telas pequenas, use `@media (min-width: …)`
  para crescer.
- Evite `!important`. Se precisou, a especificidade está errada em algum lugar.
- Unidades: `rem` para texto e espaçamento, `%` ou `fr` para layout, `px` só
  para borda.

```css
:root {
  --cor-primaria: #1f4e79;
  --cor-erro: #b3261e;
  --espaco-md: 1rem;
  --fonte-base: 1rem/1.5 system-ui, sans-serif;
}
```

## JavaScript

- `const` por padrão, `let` quando reatribuir. **Nunca** `var`.
- Nomes de função começam com verbo: `salvarAgendamento()`, `validarData()`.
- Uma função faz uma coisa. Se o nome precisa de "e" (`salvarERenderizar`),
  são duas funções.
- Nada de `onclick` no HTML; ligue eventos com `addEventListener` no JS.
- Toda validação que corresponde a uma regra de negócio vai para
  `validators.js`, com um comentário citando o ID da regra:

```js
// RN-003: preço do produto não pode ser menor ou igual a zero
function precoValido(preco) {
  return typeof preco === 'number' && preco > 0;
}
```

  Esse comentário é o que permite responder, na banca, "essa regra está
  implementada aqui" apontando a linha.
- Mensagem de erro é específica: "A data precisa ser hoje ou depois", não
  "Dados inválidos".
- Indentação de 2 espaços, ponto e vírgula sempre, aspas simples.

## Commits

Formato: `tipo: descrição no imperativo, em minúscula`

| Tipo | Quando |
|---|---|
| `feat` | Funcionalidade nova |
| `fix` | Correção de bug |
| `docs` | Só documentação |
| `style` | Formatação, CSS, sem mudar comportamento |
| `refactor` | Reorganização sem mudar comportamento |
| `chore` | Configuração, arquivo de apoio |

Exemplos: `feat: adiciona cadastro de agendamento`, `fix: corrige validação de
data no passado`, `docs: registra RN-004 e liga ao RF-002`.

Commite com frequência, ao longo do semestre. Trinta commits no dia da entrega
contam a história errada sobre o processo.

## Branches

- `main` — sempre funcionando. Nada quebrado entra aqui.
- `feat/nome-da-funcionalidade` — trabalho em andamento.
- Merge em `main` só depois de abrir o `index.html` e confirmar que roda sem erro.
