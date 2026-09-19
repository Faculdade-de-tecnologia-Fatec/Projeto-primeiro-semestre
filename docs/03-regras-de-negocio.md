# 03 — Regras de negócio

> Última atualização: 2026-09-19
> Convenção de ID: `RN-NNN`. ID nunca é reaproveitado.

## O que é (e o que não é) regra de negócio

Regra de negócio é uma restrição do **domínio**, que valeria mesmo se o sistema
fosse feito em outra linguagem, ou no papel.

| É regra de negócio | Não é (é validação de tela ou RNF) |
|---|---|
| "Não pode haver dois produtos com o mesmo código no mesmo estoque" | "O campo código é obrigatório" |
| "Agendamento só pode ser feito com no mínimo 2 horas de antecedência" | "O campo data usa o seletor nativo do navegador" |
| "Cliente inadimplente não pode abrir novo pedido" | "O botão fica cinza quando desabilitado" |

Toda RN precisa ser **testável** e ter a **exceção declarada** (mesmo que a
exceção seja "nenhuma").

## Catálogo

| ID | Regra | Exceção | Origem | RF ligadas | Status |
|---|---|---|---|---|---|
| RN-001 | `[A DEFINIR]` | | | | Proposto |

## Detalhamento

Uma seção por regra, no formato do template
[`templates/template-regra-de-negocio.md`](templates/template-regra-de-negocio.md).

### RN-001 — `[A DEFINIR]`

- **Descrição:** —
- **Quando se aplica:** —
- **O que acontece se for violada:** —
- **Exceções:** —
- **Origem:** —
- **Implementada em:** —
- **Como testar:** —

## Perguntas de lacuna

Passe esta lista sobre o domínio toda vez que uma funcionalidade nova aparecer.
Cada "sim" costuma gerar pelo menos uma RN.

- Existe cadastro? Então: o que caracteriza **duplicidade**? Pode existir
  registro repetido?
- Existe exclusão? Então: é **lógica** (marca como inativo) ou **física**
  (some)? Pode excluir algo que está sendo usado por outro registro?
- Existe data? Então: pode ser no passado? No futuro? Tem limite?
- Existe valor numérico? Então: pode ser zero? Negativo? Tem teto?
- Existe status? Então: quais transições são **proibidas**? De "concluído"
  volta para "pendente"?
- Existe listagem? Então: qual a **ordem padrão**? O que aparece quando está vazia?
- Existe mais de um perfil de usuário? Então: o que um pode fazer que o outro não?
- Existe algo que depende de outro registro? Então: o que acontece com o filho
  quando o pai some?
