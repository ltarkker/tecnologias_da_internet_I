# Tecnologias da Internet I

Repositório de trabalho da unidade curricular **Tecnologias da Internet I (TINT1)** — Licenciatura em Engenharia Informática, ISTEC Porto, ano lectivo 2026/2027.

| Item | Detalhe |
|---|---|
| Instituição | ISTEC Porto — Instituto Superior de Tecnologias Avançadas do Porto |
| Curso | Licenciatura em Engenharia Informática (LEI) |
| Ano / Semestre | 1.º ano / 1.º semestre |
| ECTS | 4 |
| Horas de contacto | 60 (48 TP + 12 OT) |
| Docente | Mário Amorim — mario.amorim@my.istec.pt |
| Estudante | Gonçalo Fernandes (2022148) |
| Plataforma | Moodle (eventos a rosa = entrega de ficha; a azul = matéria e informações) |

## Documentação

| Documento | Conteúdo |
|---|---|
| [docs/plano-e-avaliacao.md](docs/plano-e-avaliacao.md) | Planificação das aulas, regras de avaliação, datas-chave e entregas |
| [docs/ambiente-e-ferramentas.md](docs/ambiente-e-ferramentas.md) | VS Code, Live Server, Emmet, DevTools, validador do W3C e Git |
| [docs/resumo-T01.md](docs/resumo-T01.md) | T01 — a Web, o modelo cliente-servidor e o primeiro documento HTML5 |
| [docs/resumo-T02.md](docs/resumo-T02.md) | T02 — HTML5 semântico: estrutura, texto, listas, tabelas e conteúdo embebido |
| [docs/praticas.md](docs/praticas.md) | Fichas PL01 e PL02: objectivos, entregas, listas de verificação e estado do meu trabalho |
| [docs/glossario.md](docs/glossario.md) | Termos e siglas da UC |

Cada pasta de entrega tem também o seu `README.md` ([PL01](03_Trabalho_Pratico/Proj_Aulas/PL01_2022148GoncaloFernandes/README.md), [PL02](03_Trabalho_Pratico/Proj_Aulas/PL02_2022148GoncaloFernandes/README.md)).

## Objectivos da UC

- Estruturar páginas web com marcação semântica HTML5.
- Aplicar seletores e propriedades CSS3 e construir layouts responsivos com Flexbox, Grid e media queries.
- Usar JavaScript (ES6+): tipos, operadores, estruturas de controlo, arrays e funções.
- Manipular o DOM e responder a eventos do utilizador.
- Integrar as APIs do HTML5: Web Storage e geolocalização.
- Implementar comunicação assíncrona com a Fetch API (Promises e `async`/`await`), com tratamento de erros e estados de carregamento.
- Colaborar em projectos de grupo na produção de conteúdos para a Web.

## Estrutura do repositório

```
tecnologias_da_internet_I/
├── 00_FUC/                      Ficha da UC (apresentação) e planificação
├── 01_Teoricas/                 Diapositivos das aulas teóricas (T01, T02) e exemplos
│   └── t02-exemplos/            Ficheiros de exemplo da T02 (semântica, texto, listas, tabelas, media)
├── 02_Praticas/                 Enunciados das práticas laboratoriais (PL01, PL02)
│   ├── LEI-A1-S1-TINT1-PL01/    Ficha PL01 em .docx e versão revista das respostas
│   └── pl02-ficheiros/          Ficheiros de partida da PL02 (divs, tabela partida, media)
├── 03_Trabalho_Pratico/
│   ├── Proj_Aulas/
│   │   ├── PL01_2022148GoncaloFernandes/   Entrega da PL01
│   │   └── PL02_2022148GoncaloFernandes/   Entrega da PL02 (repositório Git próprio, ver nota)
│   ├── Diag.01_07.10.txt        Respostas à ficha diagnóstica da T01
│   └── Diag.02_21.10.txt        Respostas à revisão da T01 (início da T02)
├── 04_Avaliacao/                Actividades de avaliação (AA I e AA II), por preencher
├── docs/                        Documentação da UC (ver tabela acima)
└── TDII_07.txt                  Notas da aula de apresentação (07/10/2026)
```

O material do docente (diapositivos em PDF, enunciados, exemplos e ficheiros de partida) está versionado neste repositório para consulta offline. A fonte oficial continua a ser o Moodle.

**Nota sobre a PL02:** a pasta `PL02_2022148GoncaloFernandes` contém o seu próprio `.git`, ligado a [github.com/ltarkker/PL02_2022148GoncaloFernandes](https://github.com/ltarkker/PL02_2022148GoncaloFernandes). O `index.html` está também seguido pelo repositório principal. Ver [docs/ambiente-e-ferramentas.md](docs/ambiente-e-ferramentas.md#git-neste-repositório) para os cuidados a ter.

## Estado das entregas

| Ficha | Data no ficheiro | Estado | Observações |
|---|---|---|---|
| Diagnóstico 01 | 07/10/2026 | Feito | Não conta para a nota |
| PL01 | 14/10/2026 | Entregue | `index.html` validado com 0 erros (`validador.png`); respostas em `.docx` |
| Diagnóstico 02 | 21/10/2026 | Feito | Revisão da T01 |
| PL02 | 21/10/2026 | Em curso | `index.html` segue os exemplos da T02; faltam vários itens do enunciado (ver [docs/praticas.md](docs/praticas.md#estado-do-meu-trabalho-pl02)) |
| PL03 | — | Por fazer | Formulários e CSS3 |

## Planificação

| Data | Tema | Recursos | Avaliação |
|---|---|---|---|
| 07/10 | Apresentação e setup — evolução da Web, cliente-servidor, estrutura HTML5 | T01 / PL01 | Diagnóstica |
| 14/10 | HTML5 semântico — estrutura, texto, tabelas e conteúdo embebido | T02 / PL02 | |
| 21/10 | Formulários e CSS3 — formulários, validação, seletores e box model | T03 / PL03 | |
| 28/10 | Layout com CSS3 — texto, background, posicionamento e Flexbox | T04 / PL04 | |
| 04/11 | Grid e responsive — Grid Layout, media queries e acessibilidade | T05 / PL05 | |
| 11/11 | TP01 — enunciado e desenvolvimento em aula (4h) | TP01 | Enunciado AA I |
| 18/11 | TP01 — apresentações (10 min por estudante) | TP01 | AA I (30%) |
| 25/11 | JavaScript ES6+ — tipos, operadores, controlo, arrays e funções | T06 / PL06 | |
| 02/12 | Objetos e DOM — objetos, DOM, eventos e Web Storage | T07 / PL07 | Grupos e tema AA II |
| 09/12 | JavaScript assíncrono — Promises, async/await, Fetch, JSON e geolocalização | T08 / PL08 | Fecho dos grupos |
| 16/12 | TP02 — enunciado e desenvolvimento em aula (4h) | TP02 | Enunciado AA II |
| 20/01 | TP02 — apresentações (10 min por grupo) | TP02 | AA II (50%) |

As datas são as da planificação oficial. Pelos ficheiros, a PL01 foi concluída a 14/10 e a T02/PL02 a 21/10, ou seja, com uma semana de desfasamento.

## Avaliação em resumo

- **Avaliação contínua (40%)**: actividades práticas de aula 20%, Actividade de Avaliação I 30% (página responsiva, individual), Actividade de Avaliação II 50% (projecto web em grupo de 2 a 3).
- **Exame final (60%)**: Parte I teórico-prática 60% (12 valores, obrigatória, mínimo de 8 valores) e Parte II prática 40% (8 valores). Quem realizar avaliação contínua fica dispensado da Parte II.

Regras completas, datas e formato das entregas em [docs/plano-e-avaliacao.md](docs/plano-e-avaliacao.md).

## Começar

1. Instalar o [Visual Studio Code](https://code.visualstudio.com/) com a extensão **Live Server**.
2. Abrir a pasta de uma prática no VS Code (ex.: `03_Trabalho_Pratico/Proj_Aulas/PL02_2022148GoncaloFernandes`).
3. Botão direito em `index.html` → **Open with Live Server** (abre em `http://127.0.0.1:5500`).
4. Validar em [validator.w3.org](https://validator.w3.org/) por **File Upload** (o validador não chega ao Live Server) até ter 0 erros. Na PL02 activar a opção **outline**.
5. Entregar no Moodle até ao fim da aula, no formato `PLxx_<número>_<nome>.zip`.

Detalhes e atalhos em [docs/ambiente-e-ferramentas.md](docs/ambiente-e-ferramentas.md).

## Referências

- Abreu, L. (2015). *HTML 5* (4.ª ed.). FCA.
- Flanagan, D. (2020). *JavaScript: The Definitive Guide* (7.ª ed.). O'Reilly Media.
- Haverbeke, M. (2018). *Eloquent JavaScript* (3.ª ed.). No Starch Press.
- Remoaldo, P. (2011). *CSS 3*. FCA.
- Duckett, J. (2011). *HTML and CSS: Design and Build Websites*. Wiley.
- [MDN Web Docs](https://developer.mozilla.org)
- [web.dev](https://web.dev)
- [Can I Use](https://caniuse.com)
- [W3C Web Accessibility Initiative (WAI)](https://www.w3.org/WAI/)
