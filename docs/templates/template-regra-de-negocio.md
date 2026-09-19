# Template — Regra de negócio

Copie o bloco abaixo para `03-regras-de-negocio.md` e preencha. Use o próximo ID
livre; nunca reaproveite um ID.

---

### RN-NNN — Título curto e afirmativo

- **Descrição:** a regra em uma frase, no presente, afirmando o que vale.
  Ex.: *"Um agendamento só pode ser criado com no mínimo 2 horas de antecedência."*
- **Quando se aplica:** em que momento o sistema verifica isso.
  Ex.: *"Ao enviar o formulário de novo agendamento e ao editar a data de um existente."*
- **O que acontece se for violada:** o comportamento exato, incluindo a mensagem
  mostrada ao usuário, entre aspas.
- **Exceções:** os casos em que a regra não vale. Se não houver, escreva
  **"Nenhuma"** — deixar em branco é diferente de não ter exceção.
- **Origem:** de onde veio a regra (enunciado da disciplina, decisão da equipe em
  reunião de DD/MM, arquivo X do Drive). Regra sem origem é regra inventada.
- **RF ligadas:** RF-NNN, RF-NNN
- **Implementada em:** `assets/js/validators.js:NN` — ou `Ainda não implementada`
- **Como testar:** passo a passo curto que prova que a regra funciona.
- **Status:** Proposta | Aprovada | Implementada | Cancelada

---

## Teste rápido de qualidade

Antes de dar a regra por pronta:

- [ ] Ela seria verdade mesmo se o sistema fosse feito em papel? (Se não, é
      validação de tela, não regra de negócio)
- [ ] Dá para escrever um teste que a prova? (Se não, está vaga demais)
- [ ] A exceção está declarada, nem que seja "Nenhuma"?
- [ ] Está ligada a pelo menos um RF? (Regra órfã é sinal de escopo mal pensado)
