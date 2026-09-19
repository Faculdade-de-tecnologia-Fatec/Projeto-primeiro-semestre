# 02 — Requisitos

> Última atualização: 2026-09-19
> Convenção de ID: `RF-NNN` funcional, `RNF-NNN` não funcional. ID nunca é
> reaproveitado — requisito morto vira `Status: Cancelado`.

## Legenda

**Prioridade (MoSCoW):** `M` Must (sem isso não entrega) · `S` Should (importante,
mas a entrega sobrevive) · `C` Could (se sobrar tempo) · `W` Won't (fora deste semestre)

**Status:** `Proposto` → `Aprovado` → `Em desenvolvimento` → `Concluído` · `Cancelado`

## Requisitos funcionais

| ID | Requisito | Ator | Prioridade | RN ligadas | Status |
|---|---|---|---|---|---|
| RF-001 | `[A DEFINIR]` | | M | | Proposto |

> Regra de escrita: comece com verbo no infinitivo e diga o resultado observável.
> Bom: *"Cadastrar um agendamento informando cliente, serviço, data e hora."*
> Ruim: *"Tela de cadastro."* (isso é interface, não requisito)

## Requisitos não funcionais

Todo RNF precisa de critério **mensurável**. "Rápido" não é critério; "carrega em
até 3 segundos em conexão 4G" é.

| ID | Requisito | Critério de verificação | Prioridade | Status |
|---|---|---|---|---|
| RNF-001 | A interface deve ser responsiva | Layout íntegro e usável em 360px, 768px e 1280px de largura | M | Proposto |
| RNF-002 | A interface deve ser acessível | Todo `img` com `alt`; todo `input` com `label`; contraste de texto ≥ 4.5:1; navegação completa por teclado | M | Proposto |
| RNF-003 | A aplicação deve rodar sem instalação | Abrir `index.html` no navegador funciona, sem servidor e sem erro no console | M | Proposto |
| RNF-004 | Compatibilidade de navegador | Funciona em Chrome, Firefox e Edge nas versões atuais | S | Proposto |
| RNF-005 | Persistência local dos dados | Dados sobrevivem ao fechar e reabrir o navegador *(suposição — depende da decisão de usar `localStorage`)* | S | Proposto |

## Rastreabilidade

Preenchido a cada revisão. Serve para achar requisito órfão.

| RF | Regras de negócio | User stories | Onde está no código |
|---|---|---|---|
| RF-001 | — | — | — |

## Perguntas abertas

Movidas para [10-pendencias-e-melhorias.md](10-pendencias-e-melhorias.md) quando
viram ação.

- Qual é o tema do projeto?
- A disciplina exige alguma tecnologia ou formato específico de entrega?
- O trabalho é em grupo? Quantos integrantes?
