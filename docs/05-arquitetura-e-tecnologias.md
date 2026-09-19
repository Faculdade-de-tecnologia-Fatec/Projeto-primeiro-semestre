# 05 — Arquitetura e tecnologias

> Última atualização: 2026-09-19

## Stack

| Camada | Tecnologia | Motivo |
|---|---|---|
| Estrutura | HTML5 semântico | Exigência/adequação ao 1º semestre; acessibilidade sai de graça |
| Estilo | CSS3 puro (Flexbox + Grid, variáveis em `:root`) | Sem dependência externa; a banca vê o CSS que vocês escreveram |
| Comportamento | JavaScript ES6+ (sem framework) | Foco em fundamentos, que é o que a disciplina avalia |
| Persistência | `localStorage` *(suposição — confirmar)* | Dados sobrevivem ao reload sem precisar de backend |
| Versionamento | Git + GitHub | Histórico do processo, que conta na avaliação |

> ⚠️ A stack acima é a premissa de trabalho declarada pelo time. Confirmar contra
> o enunciado da disciplina assim que ele entrar na pasta do Drive.

## Estrutura de pastas proposta

```
/
├── index.html              Página principal
├── pages/                  Demais páginas HTML
├── assets/
│   ├── css/
│   │   ├── reset.css       Normalização
│   │   ├── variables.css   Cores, fontes, espaçamentos em :root
│   │   └── style.css       Estilos da aplicação
│   ├── js/
│   │   ├── main.js         Inicialização e ligação dos eventos
│   │   ├── storage.js      Leitura/escrita no localStorage
│   │   └── validators.js   Validações e regras de negócio
│   └── img/
└── docs/                   Esta documentação
```

Motivo da separação de `storage.js` e `validators.js`: as **regras de negócio**
ficam isoladas da manipulação de tela. Isso torna possível apontar, na
apresentação, exatamente onde cada RN do documento [03](03-regras-de-negocio.md)
está implementada — que é uma das perguntas mais prováveis da banca.

## Fluxo de dados

```
[ Formulário HTML ]
        │  submit
        ▼
[ main.js ] ──── valida ───▶ [ validators.js ]  (aplica as RN)
        │                            │
        │  ◀──── erro / ok ──────────┘
        ▼
[ storage.js ] ──── grava ───▶ [ localStorage ]
        │
        ▼
[ Renderiza a lista de volta na tela ]
```

## Decisões de arquitetura (ADR)

Registro curto de cada decisão relevante. Nunca apague uma decisão revogada —
marque como substituída. O histórico é o que prova amadurecimento do projeto.

| # | Data | Decisão | Alternativas consideradas | Motivo | Status |
|---|---|---|---|---|---|
| ADR-01 | 2026-09-19 | Documentação versionada no repositório, em Markdown, em vez de um documento único no Drive | Doc único no Google Docs | Histórico datado por commit, e a documentação evolui junto com o código | Aceita |
| ADR-02 | `[A DEFINIR]` | | | | Proposta |

## Diagramas

A produzir quando o escopo fechar:

- [ ] Diagrama de casos de uso (atores × funcionalidades)
- [ ] Fluxograma do processo principal
- [ ] Wireframes das telas (podem ser fotos de rascunho em papel — basta subir no Drive)
- [ ] Modelo de dados, ainda que sejam só os objetos do `localStorage`
