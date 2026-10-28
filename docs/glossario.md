# Glossário

Termos e siglas usados na UC, por ordem alfabética. Fontes: T01, T02, PL01, PL02 e FUC.

| Termo | Significado |
|---|---|
| AA I / AA II | Actividades de Avaliação I (página responsiva, 30%) e II (projecto em grupo, 50%). Também designadas TP01 e TP02. |
| AC | Avaliação contínua: 40% da nota final. |
| `alt` | Atributo obrigatório de `<img>`: descreve a imagem a quem não a vê. |
| ARPANET | Rede de 1969 que dá origem à Internet. |
| Caminho absoluto | Endereço completo, com protocolo e domínio: `https://istec-porto.pt`. |
| Caminho relativo | Caminho a partir da pasta do `index.html`: `img/avatar.png`, `sobre.html`, `../index.html`. |
| CERN | Laboratório onde Tim Berners-Lee propôs a Web (1989). O primeiro website, `info.cern.ch`, continua online. |
| Cliente-servidor | Modelo da Web: o navegador (cliente) pede, o servidor responde. Um pedido por recurso, sem memória entre pedidos. |
| Content-Type | Cabeçalho da resposta HTTP que diz o tipo do recurso, por exemplo `text/html; charset=UTF-8`. |
| CSS | Cascading Style Sheets. Apresentação: como se vê. CSS1 em 1996. |
| DevTools | Ferramentas do navegador (F12): Elements mostra o DOM; Network mostra os pedidos HTTP. |
| DNS | Domain Name System. Traduz um nome de domínio num endereço IP. |
| DOCTYPE | `<!DOCTYPE html>`: primeira linha do documento; diz ao navegador que é HTML5. |
| DOM | Document Object Model. A árvore que o navegador constrói a partir do HTML; manipula-se com JavaScript. |
| EF | Exame final: 60% da nota. Parte I teórico-prática (obrigatória, mínimo 8 valores) e Parte II prática. |
| Elemento vazio | Elemento sem conteúdo nem etiqueta de fecho: `<img>`, `<br>`, `<meta>`, `<source>`. |
| Emmet | Abreviaturas do VS Code que geram HTML: `!` + Tab gera o documento mínimo; `ul>li*3` gera uma lista. |
| Entidade | Código para escrever caracteres especiais: `&lt;`, `&gt;`, `&amp;`, `&quot;`, `&copy;`, `&nbsp;`. |
| Fragmento | Parte do URL depois de `#`: aponta para um elemento com `id`. Não é enviado ao servidor. |
| FUC | Ficha da Unidade Curricular: objectivos, método de avaliação e referências. |
| HTML | HyperText Markup Language. Estrutura: diz o que cada coisa é. |
| HTML5 / HTML Living Standard | HTML5 foi recomendação do W3C em 2014; desde 2019 a norma única é o HTML Living Standard, mantido pelo WHATWG. |
| HTTP | HyperText Transfer Protocol. Pedido do cliente (`GET /index.html`) e resposta do servidor (código de estado + recurso). |
| HTTPS | HTTP com ligação cifrada (TLS). |
| Internet | A rede mundial de redes (TCP/IP). Transporta a Web e outros serviços. |
| JavaScript | Comportamento: o que acontece na página. Criado em 1995. ES6+ nesta UC. |
| Live Server | Extensão do VS Code que serve a página em `http://127.0.0.1:5500` e a recarrega ao guardar. |
| Loopback / 127.0.0.1 | Endereço do próprio computador. Por isso o validador do W3C não chega ao Live Server. |
| Moodle | Plataforma onde estão os materiais e onde se entregam as fichas. |
| Mosaic | NCSA Mosaic, 1993: o navegador gráfico que popularizou a Web. |
| OT | Orientação tutorial (12 das 60 horas de contacto). |
| Outline | Opção do validador que mostra o índice da página a partir dos títulos `h1`–`h6`. |
| PL | Prática laboratorial: uma ficha por aula, entregue no Moodle, 20% da AC. |
| `scope` | Atributo de `<th>`: `col` para cabeçalho de coluna, `row` para cabeçalho de linha. |
| Semântica | Escolher o elemento pelo significado (`header`, `nav`, `main`, `strong`) e não pelo aspecto (`div`, `b`). |
| T | Aula teórica (T01, T02...). Os diapositivos estão em `01_Teoricas/`. |
| TCP / TLS | Protocolos de transporte e de cifra usados na ligação ao servidor. Matéria de Redes e Comunicações. |
| TP | Teórico-prática (48 das 60 horas de contacto). Também designa os trabalhos práticos TP01 e TP02. |
| URL | Uniform Resource Locator: protocolo, domínio, caminho, parâmetros e fragmento. |
| UTF-8 | Codificação de caracteres declarada em `<meta charset="UTF-8">`; sem ela os acentos aparecem mal. |
| Validador do W3C | validator.w3.org: verifica se o HTML cumpre a norma. 0 erros antes de entregar. |
| `viewport` | `<meta name="viewport" ...>`: faz a página adaptar-se ao ecrã do telemóvel. |
| W3C | World Wide Web Consortium: mantém normas da Web, entre elas a acessibilidade (WAI). |
| Web / WWW | Serviço que corre na Internet: documentos ligados por hiperligações, assente em URL, HTTP e HTML. |
| WHATWG | Grupo que mantém o HTML Living Standard. |
| Códigos de estado HTTP | 200 OK; 301 movido; 404 não encontrado; 500 erro no servidor. |
