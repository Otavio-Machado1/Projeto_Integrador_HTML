# Checklist de acessibilidade e auditoria

## Revisão estática aplicada
Os itens abaixo foram verificados no código gerado. Não equivalem a certificação de acessibilidade.

- [x] Idioma pt-BR e título descritivo por página.
- [x] Um main e um h1 por página; progressão de títulos sem saltos ascendentes.
- [x] Link de salto como primeiro elemento do body.
- [x] Menu consistente, links nativos e aria-current na página aberta.
- [x] IDs únicos e referências ARIA resolvidas.
- [x] Caminhos locais e destinos de âncoras existentes.
- [x] Imagens locais com alt que descreve função ou natureza ilustrativa.
- [x] Tabelas com caption e cabeçalhos scope.
- [x] Campos com labels; obrigatoriedade indicada em texto e por required.
- [x] Sem CSS, JavaScript ou tabindex positivo.
- [x] Formulário identificado como demonstrativo, sem cadastro real.

Os resultados automatizados constam em verificacao-estatica.csv. O script verificou propriedades estruturais; não avaliou a experiência real no navegador nem toda a conformidade do HTML.

## Testes obrigatórios ainda pendentes

### 1. Validação W3C — fazer nas quatro páginas
Acesse https://validator.w3.org/ e escolha Validate by File Upload. Envie cada HTML, corrija erros e repita.
- [ ] index.html validado.
- [ ] programacao.html validado.
- [ ] palestrantes.html validado.
- [ ] inscricao.html validado.
Registro: data / arquivo / mensagem original / correção / resultado da nova validação.
Não há resultado W3C executado neste pacote.

### 2. Teclado — fazer nas quatro páginas
- [ ] Tab e Shift+Tab percorrem links e controles em ordem lógica.
- [ ] O foco permanece visível com o estilo padrão do navegador.
- [ ] Enter no primeiro link leva ao main; o próximo Tab continua a partir do conteúdo.
- [ ] Menus, âncoras dos dias e link de retorno ao topo funcionam.
- [ ] Enter/Espaço abrem e fecham details/summary.
- [ ] Labels, select e checkbox funcionam com teclado.
- [ ] Envio vazio identifica campos obrigatórios; e-mail inválido recebe erro nativo.
- [ ] Com dados fictícios válidos, o formulário volta a #demonstracao sem valores nos parâmetros da URL.
Registro: navegador / versão / data / página / resultado / correção.

### 3. Leitor de tela e títulos
- [ ] Abrir com NVDA ou Narrador e percorrer títulos e regiões.
- [ ] Conferir nomes dos links e anúncio da página atual.
- [ ] Conferir alt das imagens, cabeçalhos das tabelas e rótulos do formulário.
- [ ] Conferir a hierarquia no HeadingsMap ou no código.
Registro: leitor / navegador / data / comportamento observado.

### 4. Ferramenta automática
- [ ] Executar Lighthouse Acessibilidade ou WAVE em cada página.
- [ ] Registrar pontuação/alertas e explicar ao menos dois resultados relevantes, se existentes.
- [ ] Corrigir problemas, repetir testes e registrar resultado final.
Não inventar alertas caso a ferramenta não os apresente. Ausência de alertas não comprova acessibilidade completa.

## Modelo de registro final
Página:
Data:
Ferramenta e versão:
Procedimento:
Resultado observado:
Problema encontrado:
Correção realizada:
Resultado após correção:
