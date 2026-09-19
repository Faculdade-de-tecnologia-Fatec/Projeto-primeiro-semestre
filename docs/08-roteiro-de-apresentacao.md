# 08 — Roteiro de apresentação

> Última atualização: 2026-09-19
> Ajustar o tempo total ao que o professor definir. O roteiro abaixo é calibrado
> para **10 minutos** de apresentação; se o tempo for outro, mantenha as
> proporções.

## Regra de ouro

Ensaie com cronômetro e sobre 20% do tempo. Apresentação que estoura o tempo é
cortada no meio, e o que fica de fora é sempre a parte boa do fim.

## Roteiro

| # | Bloco | Tempo | Quem | Conteúdo |
|---|---|---|---|---|
| 1 | Abertura | 0:30 | `[A DEFINIR]` | Nome do projeto, integrantes, uma frase sobre o que é |
| 2 | Problema | 1:30 | | Quem sofre, o que acontece hoje, qual o custo. **Sem falar do sistema ainda** |
| 3 | Solução | 1:00 | | O que o sistema faz, em alto nível. Ligar cada ponto de volta ao problema |
| 4 | Escopo | 1:00 | | O que entrou, o que ficou de fora e **por quê** |
| 5 | Demonstração | 3:00 | | O fluxo principal, do início ao fim, sem desvio |
| 6 | Regras de negócio | 1:00 | | 2 ou 3 regras, e **onde elas estão no código** |
| 7 | Processo | 1:00 | | Como se organizaram, maior dificuldade, como resolveram |
| 8 | Próximos passos | 0:30 | | O que faria com mais um mês (mostra que o backlog é consciente) |
| 9 | Encerramento | 0:30 | | Agradecimento e abertura para perguntas |

## Demonstração — o que mostrar e o que não mostrar

**Mostre um fluxo completo e feliz, do começo ao fim.** Escolha o caminho que
melhor representa o valor do produto e ensaie até fazer de olhos fechados.

Depois, mostre **um** caso de erro tratado. Isso impressiona mais que três
funcionalidades a mais, porque prova que vocês pensaram no usuário errando.

Não mostre: telas incompletas, funcionalidade que às vezes funciona, código
durante a demo (código tem o bloco 6 para isso).

## Plano B

A demo ao vivo falha. Tenha, antes do dia:

- [ ] GIF ou vídeo do fluxo principal gravado, em `docs/evidencias/`
- [ ] Prints de cada tela, em `docs/evidencias/`
- [ ] O projeto rodando localmente, sem depender de internet
- [ ] Os arquivos em pendrive **e** no Drive
- [ ] Testado no notebook que vai ser usado, com o cabo/adaptador do projetor

## Perguntas da banca

Respostas ensaiadas. Lista completa das perguntas prováveis em
[`.claude/skills/documentador/references/perguntas-da-banca.md`](../.claude/skills/documentador/references/perguntas-da-banca.md).

| Pergunta | Quem responde | Resposta |
|---|---|---|
| Que problema isso resolve? | `[A DEFINIR]` | |
| Por que HTML/CSS/JS puro? | | Foco do semestre é fundamento; o projeto não precisa de servidor para entregar o valor descrito no escopo |
| Me dá um exemplo de regra de negócio | | Citar uma RN de [03](03-regras-de-negocio.md) e o arquivo onde está implementada |
| O que ficou de fora e por quê? | | Ver seção "Fora do escopo" em [01](01-escopo-e-objetivos.md) |
| Qual foi a maior dificuldade? | | Abrir o [diário de bordo](07-diario-de-bordo.md) e mostrar a entrada datada |
| Uma pessoa cega consegue usar? | | Citar RNF-002 e demonstrar navegação por teclado |

## Ensaio

- [ ] Ensaio 1 — cronometrado, sozinho, cada um o seu bloco
- [ ] Ensaio 2 — completo, com transições entre integrantes
- [ ] Ensaio 3 — com alguém de fora fazendo perguntas difíceis
- [ ] Ensaio cruzado — cada integrante explica um bloco que **não** é o dele

O ensaio cruzado é o que evita o pior cenário: a banca apontar uma parte do
código e o integrante dizer "essa parte não fui eu que fiz".
