# Tecnologias da Internet I

Repositório de trabalho da unidade curricular **Tecnologias da Internet I (TINT1)** — Licenciatura em Engenharia Informática, ISTEC Porto, ano lectivo 2026/2027.

| Item | Detalhe |
|---|---|
| Instituição | ISTEC Porto — Instituto Superior de Tecnologias Avançadas do Porto |
| Curso | Licenciatura em Engenharia Informática (LEI) |
| Ano / Semestre | 1.º ano / 1.º semestre |
| ECTS | 4 |
| Horas de contacto | 60 (48 TP + 12 OT) |
| Docente | Mário Amorim |
| Estudante | Gonçalo Fernandes (2022148) |

## Objectivos da UC

- Estruturar páginas web com marcação semântica HTML5.
- Aplicar seletores e propriedades CSS3 e construir layouts responsivos com Flexbox, Grid e media queries.
- Usar JavaScript (ES6+): tipos, operadores, estruturas de controlo, arrays e funções.
- Manipular o DOM e responder a eventos do utilizador.
- Integrar as APIs do HTML5: Web Storage e geolocalização.
- Implementar comunicação assíncrona com a Fetch API (Promises e `async`/`await`), com tratamento de erros e estados de carregamento.

## Estrutura do repositório

```
tecnologias_da_internet_I/
├── 00_FUC/                 Ficha da unidade curricular e planificação
├── 01_Teoricas/            Aulas teóricas (T01, T02, ...) e exemplos
├── 02_Praticas/            Práticas laboratoriais (PL01, PL02, ...)
├── 03_Trabalho_Pratico/
│   ├── Proj_Aulas/
│   │   ├── PL01_2022148GoncaloFernandes/
│   │   └── PL02_2022148GoncaloFernandes/
│   ├── Diag.01_07.txt
│   └── Diag.02_21.10.txt
├── 04_Avaliacao/           Actividades de avaliação (AA I e AA II)
└── TDII_07.txt             Notas da aula de apresentação
```

O material de apoio do docente (diapositivos, enunciados, ficheiros de partida e exemplos) não é versionado — está disponível no Moodle.

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
| 09/12 | JavaScript assíncrono — Promises, async/await, Fetch, JSON e geolocalização | T08 / PL08 | |
| 16/12 | TP02 — enunciado e desenvolvimento em aula (4h) | TP02 | Enunciado AA II |
| 20/01 | TP02 — apresentações (10 min por grupo) | TP02 | AA II (50%) |

## Avaliação

**Avaliação contínua (40%)**

| Componente | Peso | Conteúdo |
|---|---|---|
| Actividades práticas de aula | 20% | Entregas das PL no Moodle |
| Actividade de Avaliação I | 30% | Página web responsiva (HTML5 + CSS3) |
| Actividade de Avaliação II | 50% | Projecto web em grupo (JavaScript, DOM e APIs do HTML5) |

**Exame final (60%)** — Fevereiro

| Componente | Peso | Conteúdo |
|---|---|---|
| Teórico-prática | 60% | Fundamentos de HTML5, CSS3 e JavaScript (12 valores) |
| Prática | 40% | Implementação de página e de scripts (8 valores) |

Quem realizar avaliação contínua pode prescindir da parte prática do exame.

## Ambiente de desenvolvimento

- [Visual Studio Code](https://code.visualstudio.com/) com a extensão **Live Server**
- Chrome, Edge ou Firefox actualizado (DevTools)
- [W3C Markup Validation Service](https://validator.w3.org/) para validação do HTML

### Abrir um exercício

1. Abrir a pasta da prática no VS Code (ex.: `03_Trabalho_Pratico/Proj_Aulas/PL02_2022148GoncaloFernandes`).
2. Clicar com o botão direito no `index.html` → **Open with Live Server**.
3. Validar o HTML em [validator.w3.org](https://validator.w3.org/) até ter zero erros.

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
