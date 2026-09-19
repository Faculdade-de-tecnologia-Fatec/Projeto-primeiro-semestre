# Checklist de entrega do PI

Use antes de cada entrega parcial e na entrega final. Marque o que existe de
verdade, não o que "está quase".

## Documentação

- [ ] Problema descrito em uma frase que alguém de fora entende
- [ ] Objetivo geral + 3 a 5 objetivos específicos, cada um verificável
- [ ] Escopo com uma seção explícita de **fora do escopo**
- [ ] Todo RF com ID, prioridade MoSCoW e status
- [ ] Todo RNF com critério mensurável (não "rápido", e sim "carrega em até 3s")
- [ ] Toda RN com exceção declarada e origem (de onde veio essa regra)
- [ ] Rastreabilidade: nenhuma RN órfã, nenhum RF sem US
- [ ] Glossário com os termos do domínio que a banca pode não conhecer
- [ ] Diário de bordo cobrindo o semestre inteiro, não só a última semana

## Código

- [ ] Roda abrindo o `index.html` no navegador, sem servidor e sem erro no console
- [ ] HTML semântico (`header`, `nav`, `main`, `section`, `footer`)
- [ ] Todo `<img>` com `alt`; todo `<input>` com `<label>` associado
- [ ] Responsivo: testado em 360px, 768px e 1280px
- [ ] Sem cor como única forma de transmitir informação
- [ ] Contraste de texto mínimo 4.5:1
- [ ] CSS sem `!important` espalhado; variáveis em `:root`
- [ ] JS sem `var`; funções com nome que diz o que fazem
- [ ] Validação de formulário com mensagem de erro visível e específica
- [ ] README explica como rodar em 3 linhas

## Apresentação

- [ ] Roteiro cronometrado, com folga de 20% no tempo
- [ ] Papel de cada integrante definido na apresentação
- [ ] Evidências (print/GIF) de cada funcionalidade — não dependa de demo ao vivo
- [ ] Plano B se a internet cair ou o notebook não conectar no projetor
- [ ] Respostas ensaiadas para as 5 perguntas mais prováveis da banca
- [ ] Cada integrante sabe explicar **qualquer** parte, não só a sua

## Repositório

- [ ] Commits distribuídos ao longo do semestre, não todos no último dia
- [ ] Commits de todos os integrantes (a banca olha isso)
- [ ] Mensagens de commit descritivas
- [ ] Sem arquivo de senha, `.env` ou dado pessoal versionado
