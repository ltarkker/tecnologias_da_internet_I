# PL02 — Uma página com estrutura, listas, tabelas e multimédia

Entrega da prática laboratorial 02 de Tecnologias da Internet I (ISTEC Porto, LEI, 2026/2027).

| Item | Detalhe |
|---|---|
| Estudante | Gonçalo Fernandes (2022148) |
| Data | 21/10/2026 |
| Enunciado | `../../../02_Praticas/LEI-A1-S1-TINT1-PL02.pdf` |
| Ficheiros de partida | `../../../02_Praticas/pl02-ficheiros/` |
| Resumo e lista de verificação | [docs/praticas.md](../../../docs/praticas.md#pl02--uma-página-com-estrutura-listas-tabelas-e-multimédia) |
| Repositório GitHub | https://github.com/ltarkker/PL02_2022148GoncaloFernandes |

## Ficheiros

| Ficheiro | Conteúdo |
|---|---|
| `index.html` | Página "A WEB em poucas palavras": `header` com `nav`, `main` com `article` e secções de ênfase no texto, citações, entidades HTML, listas (`ul`, `ol`, `dl`) e duas tabelas (`caption`, `thead`, `tbody`, `tfoot`, `scope`, `colspan`); `aside` com desafio; `footer`. Regra CSS no `head` para as bordas das tabelas. |
| `LEI-A1-S1-TINT1-PL02.docx` | Ficha PL02 em preenchimento (respostas aos exercícios; substitui o `respostas.txt`). Até agora só tem a resposta ao ex. 1.1. |

## Abrir

1. Abrir esta pasta no VS Code.
2. Botão direito em `index.html` → **Open with Live Server**.
3. Validar em [validator.w3.org](https://validator.w3.org/) por **File Upload**, com a opção **outline** activa.

## Estado

A página segue os exemplos da T02. Para cumprir o enunciado da PL02 faltam:

- `nav` com `ul` de quatro ligações (`#sobre`, `#plano`, `#multimedia`, `#ligacoes`) e as quatro `section` correspondentes.
- Conteúdo pessoal da PL01 (nome, avatar em `figure`, sobre mim, hobbies, ligações), `abbr` e `time`.
- Tabela do plano semanal com `rowspan` e total de 20 horas.
- `video` com dois `source`, `audio`, `iframe` do OpenStreetMap com `title` e atribuição no `footer`; pasta `media/`.
- `pl02-divs-corrigido.html`, `pl02-tabela-corrigida.html`, `respostas.txt` e `validador.png`.
- Comentário inicial com PL02, nome, número e data.

A corrigir no `index.html` actual antes de validar:

1. `li` directamente dentro de outro `li` na lista não ordenada: a sublista precisa da sua própria `ul`.
2. `</dt>` solto no fim da lista de descrição.
3. Gralhas em `aria-label="Navegação princial"` e "Para mostras os símbolos".

## Git

Esta pasta é um repositório Git próprio. O `index.html` está também seguido pelo repositório principal da UC, por isso alterações têm de ser commitadas nos dois. Ver [docs/ambiente-e-ferramentas.md](../../../docs/ambiente-e-ferramentas.md#git-neste-repositório).
