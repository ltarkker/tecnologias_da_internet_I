# PL02 — Uma página com estrutura, listas, tabelas e multimédia

Entrega da prática laboratorial 02 de Tecnologias da Internet I (ISTEC Porto, LEI, 2026/2027).

| Item | Detalhe |
|---|---|
| Estudante | Gonçalo Fernandes (2022148) |
| Data | 21/10/2026 |
| Enunciado | `../../../02_Praticas/LEI-A1-S1-TINT1-PL02.pdf` |
| Ficheiros de partida | `../../../02_Praticas/pl02-ficheiros/` |
| Resumo e lista de verificação | [docs/praticas.md](../../../docs/praticas.md#pl02--uma-página-com-estrutura-listas-tabelas-e-multimédia) |

## Ficheiros

| Ficheiro | Conteúdo |
|---|---|
| `index.html` | Página pessoal da PL02: comentário inicial (PL02, nome, número, data); `header` com `h1` e `nav` (`ul` com as quatro ligações); `main` com as `section` Sobre mim (`figure` com avatar, `abbr`, `time`, `strong`/`em`, `code`, `blockquote`, listas `ul`/`ol`/`dl` com `mark` no glossário), Plano semanal (tabela com `caption`, `thead`/`tbody`/`tfoot`, `scope`, `colspan`, `rowspan`), Multimédia (`video` com dois `source` e `poster`, `audio`, `iframe` do OpenStreetMap com `title`), Ligações e Notícias (dois `article` com `header`/`footer`, extra); `aside`; `footer` com `&copy;` e atribuição do mapa. Regra CSS no `head` para as bordas das tabelas. |
| `pl02-divs-corrigido.html` | Exercício 1: a "sopa de divs" reescrita com `header`, `nav`, `main`, `section`, `article`, `aside` e `footer`. |
| `pl02-tabela-corrigida.html` | Exercício 6: a tabela partida corrigida (`thead`/`tbody`, `scope`, `colspan="2"`). |
| `respostas.txt` | Respostas aos exercícios 1, 3, 6 e 8 e descrição dos extras. |
| `img/` | `avatar_halloween.png`, usado na `figure` do index. |
| `media/` | `apresentacao.webm`, `apresentacao.mp4`, `poster.jpg` e `som.mp3`, usados nas etiquetas `video` e `audio`. |
| `pl02-divs.html`, `pl02-tabela-partida.html` | Ficheiros de partida do enunciado (não alterados, não fazem parte da entrega). |

## Abrir

1. Abrir esta pasta no VS Code.
2. Botão direito em `index.html` → **Open with Live Server**.
3. Validar em [validator.w3.org](https://validator.w3.org/) por **File Upload**, com a opção **outline** activa.

## Estado

Entrega praticamente completa: `index.html`, `pl02-divs-corrigido.html` e `pl02-tabela-corrigida.html` validam com 0 erros e 0 avisos no validator.w3.org, e o `respostas.txt` tem os exercícios 1, 3, 6 e 8 e os extras. Falta só:

- `validador.png`: captura do validador (File Upload + opção **outline**) do `index.html`, a guardar na raiz do repositório e a incluir no zip.

## Git

Esta pasta é um repositório Git próprio. O `index.html` está também seguido pelo repositório principal da UC, por isso alterações têm de ser commitadas nos dois. Ver [docs/ambiente-e-ferramentas.md](../../../docs/ambiente-e-ferramentas.md#git-neste-repositório).