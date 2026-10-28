# Práticas laboratoriais

Enunciados em `02_Praticas/`. Entregas em `03_Trabalho_Pratico/Proj_Aulas/`. Regras gerais (entrega, IA, validação) em [plano-e-avaliacao.md](plano-e-avaliacao.md#regras-das-fichas-pl).

## Fichas diagnósticas

Não contam para a nota; servem para o docente ajustar as aulas. Respostas em `03_Trabalho_Pratico/`.

| Ficha | Data | Perguntas | Ficheiro |
|---|---|---|---|
| Diag. 01 | 07/10/2026 | O que acontece entre escrever um URL e ver a página; Internet vs Web; papel de HTML, CSS e JS; experiência prévia | `Diag.01_07.10.txt` (inclui notas da T01: cronologia, cliente-servidor, códigos HTTP, UTF-8) |
| Diag. 02 | 21/10/2026 | Revisão da T01: três linhas obrigatórias, `href` relativo vs absoluto, quantos `h1`, `img` sem `alt` | `Diag.02_21.10.txt` |

Correcção da Diag. 02 em [resumo-T02.md](resumo-T02.md#revisão-da-t01).

## PL01 — A Web por dentro e a minha primeira página HTML5

Consolida a T01. Em aula, 65 minutos, exercícios 1 a 7; extras opcionais. Enunciado: `02_Praticas/LEI-A1-S1-TINT1-PL01.pdf`.

### Objectivos

- Observar nas DevTools os pedidos e as respostas HTTP de uma página.
- Interpretar códigos de estado (200 e 404) e o Content-Type.
- Criar um documento HTML5 válido a partir do modelo do Emmet.
- Usar títulos, parágrafos, ligações, imagens e comentários.
- Ler as mensagens do validador do W3C e corrigir os erros.

### Exercícios

| # | Exercício | Tempo | Resumo |
|---|---|---|---|
| 1 | Contar pedidos HTTP | 12 min | Janela privada, DevTools > Rede, Disable cache. Comparar `info.cern.ch` com a Wikipédia: n.º de pedidos, estado, Content-Type, tipos, dados. |
| 2 | Provocar um 404 e ler o código-fonte | 8 min | `info.cern.ch/nao-existe`; página inexistente da Wikipédia (parece normal, mas é 404). Ctrl + U no CERN: etiquetas em maiúsculas, sem DOCTYPE, sem aspas, sem fecho. |
| 3 | Preparar o projecto | 5 min | `tint1/pl01/index.html` e `img/`; `!` + Tab; `lang="pt-PT"`; Go Live. |
| 4 | A minha página de apresentação | 20 min | Comentário com nome, n.º e data; ligação `#ligacoes`; um `h1`; imagem em `img/` com `alt` e `width="160"`; Sobre mim (`h2`, `br` na morada, Hobbies em `h3`); Porque escolhi EI (`h2`); Ligações (`h2 id="ligacoes"`) com duas ligações absolutas. |
| 5 | Prever e testar | 5 min | `prever.html`: o navegador junta linhas do código num só espaço; `br` quebra linha; `<br><br>` só dá espaço, não é boa prática. |
| 6 | Caça aos erros | 10 min | Seis problemas, o validador só apanha quatro (falta DOCTYPE, `h1` fechado com `h2`, `img` sem `alt`, aninhamento `</p></strong>`). Não apanha `href` sem aspas nem `<p>` por fechar. |
| 7 | Validar, inspeccionar e entregar | 5 min | File Upload até 0 erros; `validador.png`; Ctrl + U mostra o comentário, a página não. |
| Extra | `sobre.html` e ligações relativas | — | Da pasta `paginas/` volta-se com `../index.html`. Com o Live Server a página faz 4 pedidos: HTML, imagem, favicon (404) e WebSocket do Live Server. |

### Entrega

`PL01_<número>_<nome>.zip` com a pasta `pl01` (`index.html`, `prever.html`, `img/`), `respostas.txt` (tabelas dos ex. 1, 5 e 6; respostas dos ex. 1, 2, 6 e 7) e `validador.png`.

Mínimo esperado: `index.html` válido, `lang="pt-PT"`, comentário, um só `h1`, imagem com `alt`, três `h2` e um `h3`, um `br` bem usado, ligação `#ligacoes` e duas ligações externas.

### Lista de verificação

- [x] Tabela do exercício 1 preenchida
- [x] Códigos 404 e etiquetas do CERN (ex. 2)
- [x] Previsões do exercício 5 confirmadas
- [x] Seis problemas do exercício 6 explicados
- [x] Respostas do exercício 7 (URI e Ctrl + U)
- [x] Captura `validador.png` com 0 erros
- [x] `lang="pt-PT"` e `title` com o nome
- [x] Comentário com nome, número e data
- [x] Um `h1`, três `h2` e um `h3`, sem saltos
- [x] `br` na morada, sem `<br><br>`
- [x] Imagem em `img/`, com `alt` e `width`
- [x] Ligação `#ligacoes` e duas ligações externas

### Estado do meu trabalho (PL01)

Pasta `03_Trabalho_Pratico/Proj_Aulas/PL01_2022148GoncaloFernandes/`, datada de 14/10/2026 no comentário do `index.html`.

| Ficheiro | Conteúdo |
|---|---|
| `index.html` | Página de apresentação com todos os itens do exercício 4. Validada com 0 erros. |
| `prever.html` | Excerto do exercício 5, copiado sem alteração. |
| `img/avatar_halloween.png` | Avatar (952 kB; pesado para o limite do Moodle, convém comprimir em entregas futuras). |
| `validador.png` | Captura do validador. |
| `LEI-A1-S1-TINT1-PL01.docx` | Ficha preenchida com as respostas, em vez do `respostas.txt` pedido no enunciado. |

Existe uma segunda versão das respostas, mais revista e com os extras respondidos, em `02_Praticas/LEI-A1-S1-TINT1-PL01/LEI-A1-S1-TINT1-PL01_respostas.docx`. A versão na pasta de entrega não tem os extras.

Ponto a rever: a ligação interna no topo aponta para `#ligcoes` e o `h2` tem `id="ligacoes"`. Como estão escritos de forma diferente, o salto não funciona. O validador não apanha este erro.

## PL02 — Uma página com estrutura, listas, tabelas e multimédia

Consolida a T02. Em aula, 70 minutos, exercícios 1 a 8; extras opcionais. Enunciado: `02_Praticas/LEI-A1-S1-TINT1-PL02.pdf`. Ficheiros de partida em `02_Praticas/pl02-ficheiros/` (`pl02-divs.html`, `pl02-tabela-partida.html`, `media/`).

### Objectivos

- Identificar e substituir divs pelos elementos semânticos adequados.
- Organizar uma página com `header`, `nav`, `main`, `section`, `aside` e `footer`.
- Usar elementos de texto com significado, entidades e os três tipos de lista.
- Construir tabelas acessíveis, com `colspan` e `rowspan`.
- Incorporar figura, vídeo, áudio e mapa, com os ficheiros organizados.
- Validar a estrutura da página com a opção outline do validador.

### Exercícios

| # | Exercício | Tempo | Resumo |
|---|---|---|---|
| 1 | Da sopa de divs à semântica | 10 min | `pl02-divs.html` (Clube de Programação) é válido mas só tem `div`. Tabela dos 7 `div` → elemento semântico; guardar como `pl02-divs-corrigido.html`; `&copy;` no rodapé; `<time datetime="2026-10-30">` na Hackathon. |
| 2 | A estrutura da minha página | 8 min | `index.html`: comentário actualizado; `header` com `h1` e `nav` com `ul` de quatro ligações (`#sobre`, `#plano`, `#multimedia`, `#ligacoes`); um `main` com quatro `section` (Sobre mim, Plano semanal, Multimédia, Ligações); `aside` com dica; `footer` com `&copy;`, ano e nome. |
| 3 | Texto com significado | 8 min | Em Sobre mim: `abbr` para LEI e ISTEC; `time` com a data de início do curso; um `strong` e um `em` (justificar no `respostas.txt`); `<h1>` literal com `code` e entidades; `blockquote` seguido do autor. |
| 4 | Três listas | 7 min | Cada uma com `h3`: Hobbies (`ul`), três sites preferidos (`ol`), glossário de TINT1 (`dl` com três termos). |
| 5 | O plano semanal | 15 min | Tabela com `caption`; `thead` com três `th scope="col"`; dias em `th scope="row"`; quarta com `colspan="2"`; quinta/sexta com `rowspan="2"`; `tfoot` com total de 20 horas em `colspan="2"`; regra CSS `table, th, td { border: 1px solid #999; border-collapse: collapse; padding: 6px 10px; }`. |
| 6 | A tabela partida | 5 min | `pl02-tabela-partida.html`: `td` do Rui fora de `tr`; `colspan="3"` a mais. Registar mensagens do validador; guardar como `pl02-tabela-corrigida.html` com `thead`/`tbody`, `scope` e nomes em `th scope="row"`. 0 erros e 0 avisos. |
| 7 | Figura, vídeo, áudio e mapa | 12 min | Copiar `media/`. Avatar em `figure` com `figcaption`; `video controls width="400" poster` com dois `source` (webm, mp4) e texto alternativo; `audio controls` com `som.mp3`; `iframe` do OpenStreetMap com `title`; atribuição no `footer`. |
| 8 | Validar com outline e entregar | 5 min | File Upload com outline; `validador.png`; copiar o outline para o `respostas.txt`; comparar com a PL01: os elementos semânticos não mudaram o aspecto. |
| Extra | Notícias, `mark`, iframe do Google | — | Secção com dois `article` (cada um com `header` e `footer`); `mark` em cada definição; `google.com` recusa ser incorporado. |

### Tabela de referência do exercício 1

| `div` (class) | Elemento semântico | Porquê |
|---|---|---|
| topo | `header` | Cabeçalho da página: título e menu |
| menu | `nav` | Navegação principal |
| conteudo | `main` | Conteúdo principal, único |
| bloco | `section` | Tema da página com o seu `h2` |
| noticia | `article` | Faz sentido sozinho |
| lateral | `aside` | Conteúdo acessório |
| rodape | `footer` | Rodapé |

### Entrega

`PL02_<número>_<nome>.zip` com a pasta `pl02` (`index.html`, `pl02-divs-corrigido.html`, `pl02-tabela-corrigida.html`, `img/`, `media/`), `respostas.txt` (tabelas dos ex. 1 e 6; respostas dos ex. 1, 3 e 8) e `validador.png` com o outline.

Mínimo esperado: `index.html` válido com `header`, `nav` em lista, um `main` com quatro `section`, `aside` e `footer`; `abbr`, `time`, `strong` e `em`; `ul`, `ol` e `dl`; tabela com `caption`, `scope`, `colspan`, `rowspan` e `tfoot`; `figure`, `video` com dois `source`, `audio` e `iframe` com `title`.

### Estado do meu trabalho (PL02)

Pasta `03_Trabalho_Pratico/Proj_Aulas/PL02_2022148GoncaloFernandes/`, com `index.html` datado de 21/10/2026, a ficha `LEI-A1-S1-TINT1-PL02.docx` em preenchimento (a 28/10 só tem a resposta ao ex. 1.1) e repositório Git próprio publicado em GitHub (ver [ambiente-e-ferramentas.md](ambiente-e-ferramentas.md#git-neste-repositório)).

O `index.html` actual acompanha os exemplos da T02 (ênfase, citações, entidades, listas, duas tabelas com `caption`/`thead`/`tbody`/`tfoot` e `scope`) dentro de `header`, `main`, `article`, `aside` e `footer`. Em relação ao enunciado da PL02:

- [x] `header` com `h1` e `nav`
- [x] Um só `main`, `aside` e `footer`
- [x] `strong`, `em`, `mark`, `abbr`, `code`, `small`, `time`
- [x] `blockquote` e `q`; entidades `&lt;`, `&gt;`, `&amp;`, `&quot;`, `&copy;`
- [x] `ul`, `ol`, `ol type="a"` e `dl`
- [x] Tabelas com `caption`, `thead`, `tbody`, `tfoot`, `scope` e `colspan`
- [ ] `nav` com `ul` de quatro ligações (`#sobre`, `#plano`, `#multimedia`, `#ligacoes`); as ligações actuais estão soltas e apontam para `#texto`, `#citacoes` e `#entidades`
- [ ] Quatro `section` com os `id` e títulos do enunciado (Sobre mim, Plano semanal, Multimédia, Ligações)
- [ ] Conteúdo pessoal da PL01 (nome, avatar, sobre mim, hobbies, ligações)
- [ ] Tabela do plano semanal com `rowspan` e total de 20 horas
- [ ] `figure` com `figcaption`, `video` com dois `source`, `audio`, `iframe` com `title`, atribuição do OpenStreetMap
- [ ] `pl02-divs-corrigido.html` e `pl02-tabela-corrigida.html`
- [ ] `respostas.txt` e `validador.png` com outline
- [ ] Comentário inicial com PL02, nome, número e data

Pontos a corrigir antes de validar, segundo as regras da T02:

1. Na lista não ordenada, há `li` directamente dentro de outro `li`. A sublista tem de ir dentro de uma `ul` própria dentro do `li`.
2. Na lista de descrição há um `</dt>` solto depois do último `dd`.
3. Gralhas: `aria-label="Navegação princial"` e "Para mostras os símbolos".

## Próximas fichas

| Ficha | Aula | Tema |
|---|---|---|
| PL03 | 21/10 (plano) | Formulários, validação, seletores CSS e box model |
| PL04 | 28/10 | Texto, background, posicionamento e Flexbox |
| PL05 | 04/11 | Grid Layout, media queries e acessibilidade |
| PL06 | 25/11 | JavaScript ES6+: tipos, operadores, controlo, arrays e funções |
| PL07 | 02/12 | Objetos, DOM, eventos e Web Storage |
| PL08 | 09/12 | Promises, async/await, Fetch, JSON e geolocalização |
