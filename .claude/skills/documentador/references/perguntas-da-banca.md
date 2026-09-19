# Perguntas que a banca faz (e como se preparar)

Banca de PI de primeiro semestre não cobra arquitetura avançada. Ela cobra
**clareza, coerência e domínio do que vocês mesmos fizeram**. As perguntas abaixo
aparecem quase sempre. Cada uma deve ter resposta escrita em
`docs/08-roteiro-de-apresentacao.md`.

## Sobre o problema

1. Que problema real isso resolve? Quem sofre com ele hoje?
2. Como esse problema é resolvido hoje, sem o sistema de vocês?
3. Por que essa solução é melhor que a planilha que a pessoa já usa?

> Armadilha: responder com a funcionalidade em vez do problema. "Nosso sistema
> cadastra produtos" não é problema, é solução. O problema é o que dói antes.

## Sobre o escopo

4. O que ficou de fora e por quê?
5. Se tivessem mais um mês, o que fariam primeiro?
6. Como vocês decidiram a prioridade das funcionalidades?

> Armadilha: dizer "não deu tempo". Diga "priorizamos X porque Y; Z ficou no
> backlog como Should". Corte consciente é maturidade; corte por atraso é falha.

## Sobre as regras de negócio

7. Me dá um exemplo de regra de negócio do sistema de vocês.
8. O que acontece se o usuário tentar [caso de erro óbvio do domínio]?
9. Essa regra está implementada ou só documentada?

> Armadilha: confundir regra de negócio com validação de tela. "O campo é
> obrigatório" é validação. "Não pode haver dois produtos com o mesmo código no
> mesmo estoque" é regra de negócio.

## Sobre o código

10. Quem escreveu esta parte? Explica o que ela faz.
11. Por que HTML/CSS/JS puro e não um framework?
12. Onde ficam os dados quando a página é fechada?
13. O que acontece se eu apertar esse botão duas vezes rápido?

> Armadilha: um integrante não saber explicar o trecho que a banca apontou.
> Ensaie com cada um explicando uma parte que **não** foi ele quem escreveu.

## Sobre o processo

14. Como vocês se organizaram? Com que frequência se reuniam?
15. Qual foi a maior dificuldade e como resolveram?
16. O que vocês fariam diferente?

> Aqui o diário de bordo salva. Abrir o `07-diario-de-bordo.md` e mostrar o
> histórico datado responde 14 e 15 de uma vez.

## Sobre acessibilidade e usabilidade

17. Uma pessoa cega consegue usar isso?
18. Funciona no celular?
19. Como o usuário sabe que deu erro?

> Essas três valem nota fácil e quase sempre são esquecidas. `alt`, `label`,
> navegação por teclado, contraste e mensagem de erro específica.
