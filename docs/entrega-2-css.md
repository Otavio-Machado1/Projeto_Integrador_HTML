# Entrega 2: estilos e responsividade

O CSS fica em `estilo.css`, na raiz, ligado às quatro páginas por `<link rel="stylesheet">`. Os comentários do arquivo indicam a etapa de cada regra.

## O que veio de cada aula

| Aula | Etapas | Aplicação na SATEC |
| --- | --- | --- |
| 13 | 1 a 6 | Cores, fontes, cabeçalho, rodapé, especificidade e ordem da cascata |
| 15 | 7 a 12 | `box-sizing: border-box`, `.botao` em inline-block, menus e cards em Flexbox, `.cards` com `repeat(auto-fit, minmax(220px, 1fr))`, mapa da página com `grid-template-areas` |
| 16 | 13 a 16 | Formulário com `fieldset`, `legend` e `div.campo`; `:focus-visible` e `:user-invalid`; media queries mobile first; cabeçalho em Grid e menu em Flexbox |
| 17 | 17 a 22 | Variáveis no `:root`, modo escuro com `light-dark()`, `clamp()`, `text-wrap`, `color-mix()`, nesting, `:has()`, container query e `prefers-reduced-motion` |

O Tailwind (etapas 23 e 24) não foi usado. A aula trata o tema como conteúdo extra, e ele exigiria um script externo.

## Larguras

| Largura | Layout |
| --- | --- |
| Base (celular) | Uma coluna: topo, conteúdo, lateral e rodapé empilhados; menu em botões que preenchem a linha |
| 600px ou mais | Dois campos por linha no formulário; menu numa linha; rodapé em duas colunas |
| 900px ou mais | O `aside` sobe para a lateral de 280px; logo, menu e botão lado a lado no cabeçalho |

A lista "Informações rápidas" usa container query. Ela fica com termo e valor lado a lado quando o `aside` tem 30rem ou mais, e empilhada na lateral estreita do desktop.

## Mudanças no HTML

- Classes para o layout: `pular`, `logo`, `aviso`, `botao`, `cards`, `card`, `palestrante`, `nota`, `campo`, `aceite`, `dica`.
- Link "Inscreva-se" no cabeçalho, com cara de botão, mas continua sendo `<a>`.
- `div.cards` agrupa os cards só para o Grid, sem significado.
- Formulário dividido em "Dados pessoais" e "Dados acadêmicos" com `fieldset` e `legend`; dica do e-mail ligada por `aria-describedby`.
- Em `programacao.html`, um texto de comentário que aparecia na página voltou a ser comentário.

## Decisões

- As ilustrações dos palestrantes têm texto na parte de baixo. Por isso não viraram círculos com `border-radius: 50%`, como no gabarito da aula.
- O botão usa `--cor-botao`, igual nos dois temas, para o texto branco continuar legível no modo escuro.
- O `main` com `tabindex="-1"` perde o contorno só no clique (`:focus:not(:focus-visible)`); pelo teclado o contorno aparece.

## Conferência feita

As quatro páginas foram abertas no Edge em 375px e 1280px, nos temas claro e escuro. Não houve rolagem horizontal nem erro de carregamento.
