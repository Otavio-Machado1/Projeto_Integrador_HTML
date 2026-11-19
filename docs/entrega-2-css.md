# Entrega 2: estilos e responsividade

O CSS fica em `estilo.css`, na raiz, e usa só recursos mostrados nas aulas 15, 16 e 17.

| Aula | Aplicação na SATEC |
| --- | --- |
| 15 | `box-sizing: border-box`, `.botao` em inline-block, cabeçalho e menus em Flexbox, `.cards` com `repeat(auto-fit, minmax(220px, 1fr))`, mapa da página com `grid-template-areas` |
| 16 | Formulário com `fieldset`, `legend` e `div.campo`; `:focus-visible`, `:user-invalid`, `:has()`, `:not()`, `:nth-child(even)`; media queries começando pelo celular |
| 17 | Variáveis no `:root` e `clamp()` no `h1` |

| Largura | Layout |
| --- | --- |
| Base (celular) | Uma coluna: topo, conteúdo, lateral e rodapé empilhados |
| 600px ou mais | Menu numa linha e dois campos por linha no formulário |
| 900px ou mais | O `aside` vai para a lateral de 280px |

O HTML da entrega 1 foi mantido. Ele recebeu apenas o `<link>` do CSS, as classes `pular`, `botao`, `cards`, `palestrante`, `campo`, `dica` e `aceite`, o link "Inscreva-se" no cabeçalho e os grupos `fieldset` do formulário, como no material das aulas.
