# Template — User story

Copie o bloco abaixo para `04-backlog.md`.

---

### US-NNN — Título curto

> Como **`<ator>`**, quero **`<ação>`**, para **`<benefício>`**.

- **Épico:** EP-NN
- **RF atendidos:** RF-NNN
- **RN envolvidas:** RN-NNN
- **Prioridade:** M | S | C | W
- **Estimativa:** P | M | G
- **Sprint:** N
- **Status:** Proposta | Em desenvolvimento | Concluída | Cancelada

**Critérios de aceite**

- [ ] **Dado** que `<contexto>`, **quando** `<ação do usuário>`, **então**
      `<resultado observável>`.
- [ ] **Dado** que `<contexto>`, **quando** `<ação>`, **então** `<resultado>`.
- [ ] **Erro:** **dado** que `<contexto inválido>`, **quando** `<ação>`, **então**
      o sistema exibe `"<mensagem exata>"` e não grava nada.
- [ ] **Vazio:** **dado** que não há registro nenhum, **quando** a tela abre,
      **então** o sistema mostra `"<mensagem de estado vazio>"`.

**Definição de pronto**

- [ ] Critérios de aceite verificados no navegador
- [ ] Sem erro no console
- [ ] Funciona em 360px, 768px e 1280px
- [ ] Campos com `label`; mensagens de erro específicas
- [ ] Evidência em `docs/evidencias/`
- [ ] Documentação atualizada e commitada

---

## Teste rápido de qualidade

- [ ] O "para `<benefício>`" foi escrito sem esforço? (Se não saiu, a história
      talvez não devesse existir)
- [ ] O ator é uma pessoa real do domínio, não "o usuário" genérico?
- [ ] Há pelo menos um critério de **erro** e um de **estado vazio**? São os dois
      mais esquecidos e os que a banca testa primeiro
- [ ] Dá para entregar isso em um único sprint? Se não, quebre em duas
