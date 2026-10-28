# Ambiente e ferramentas

Fonte: T01, diapositivos 19 a 25, 31 e 36; T02, diapositivos 24 e 26.

## O que se usa todas as semanas

| Ferramenta | Para quê | Como abrir |
|---|---|---|
| Visual Studio Code | Escrever HTML, CSS e JavaScript | `code .` na pasta do projecto |
| Navegador + DevTools | Ver o que o navegador vê; pedidos HTTP, DOM | F12 |
| Validador do W3C | Confirmar que o HTML cumpre a norma. 0 erros antes de entregar | [validator.w3.org](https://validator.w3.org/) |
| Git + GitHub | Histórico do trabalho. Útil já nos TP | `git commit` |

Confirmar a instalação no terminal:

```powershell
code --version
git --version
```

## VS Code

### Extensões e definições recomendadas

- **Live Server**: abre a página em `http://127.0.0.1:5500` e recarrega-a sempre que se guarda. Instalar uma vez em Extensions (Ctrl + Shift + X).
- **Prettier**: formata o código de forma consistente.
- **Auto Save** (File > Auto Save): deixa de ser preciso Ctrl + S.
- **Linked Editing** (`"editor.linkedEditing": true`): ao mudar a etiqueta de abertura, a de fecho acompanha.
- **Emmet**: já vem incluído.

### Atalhos

| Atalho | Efeito |
|---|---|
| `!` + Tab | Gera o modelo HTML5 (Emmet) |
| Ctrl + S | Guardar |
| Shift + Alt + F | Formatar o documento |
| Ctrl + / | Comentar ou descomentar a linha |
| Ctrl + G | Ir para a linha (útil com as mensagens do validador) |

### Emmet

| Escreves | Obténs |
|---|---|
| `!` | Documento HTML5 completo (mudar `lang="en"` para `pt-PT` e o `title`) |
| `h1` | `<h1></h1>` |
| `p*2` | dois `<p></p>` |
| `a` | `<a href=""></a>` |
| `img` | `<img src="" alt="">` |
| `br` | `<br>` |
| `ul>li*3` | lista com três itens |

Se nada acontecer, confirmar que o ficheiro termina em `.html` (canto inferior direito: HTML).

## Criar um projecto

Pelo terminal (PowerShell):

```powershell
cd Documents
mkdir tint1\pl01\img
cd tint1\pl01
code .
```

Ou pelo VS Code: File > Open Folder, depois New File (`index.html`) e New Folder (`img`).

Regras de organização (T01 diap. 24, T02 diap. 24):

- A página principal chama-se sempre `index.html`. A extensão `.html` é obrigatória.
- Nomes em minúsculas, sem espaços nem acentos, com hífen: `foto-perfil.jpg`, `apresentacao.mp4`.
- Uma pasta por tipo: `img/` para imagens, `media/` para vídeo e áudio.
- Caminhos relativos (`img/avatar.png`, `media/som.mp3`), nunca caminhos do disco (`C:\Users\...`).
- Ficheiros leves: o Moodle tem limite de tamanho.
- Direitos de autor: conteúdos próprios ou com licença livre, com a fonte indicada.

```
pl02/
├── index.html
├── img/
│   └── avatar.png
└── media/
    ├── apresentacao.mp4
    ├── apresentacao.webm
    └── som.mp3
```

## Navegador e DevTools

| Atalho | Efeito |
|---|---|
| F12 | Abre as DevTools |
| Ctrl + U | Código-fonte: o HTML tal como veio do servidor |
| F12 > Elements | A árvore DOM que o navegador construiu |
| F12 > Network (Rede) | Um pedido por recurso: estado, tipo, Content-Type, tamanho |
| Ctrl + Shift + N (Firefox: Ctrl + Shift + P) | Janela privada: sem extensões nem sessão |
| Disable cache (em Rede) | Obriga a pedir tudo de novo ao servidor |

O que procurar no separador Rede: `Status 200`, `Type document`, `Content-Type text/html`, número de pedidos.

## Validador do W3C

| Modo | Quando |
|---|---|
| Validate by URI | Página publicada na Internet. **Não funciona com o Live Server**: `127.0.0.1` só existe no próprio computador, e o validador corre num servidor remoto. |
| Validate by File Upload | Enviar o `index.html`. É o modo usado nas entregas. |
| Validate by Direct Input | Colar um excerto de código. Útil para testar. |

Como ler uma mensagem:

```
Error: An "img" element must have an "alt" attribute, except under certain conditions.
From line 10, column 3; to line 10, column 26
```

- **Error**: tem de ser corrigido; conta para o 0 erros.
- **Warning**: aviso; ler e decidir, não impede a entrega.
- `line 10`: ir a essa linha no VS Code (Ctrl + G).
- Corrigir sempre o primeiro erro e validar de novo: um só erro pode gerar várias mensagens.

Opção **Show: outline** (T02): mostra o índice da página a partir dos títulos. Se o índice não fizer sentido, a hierarquia `h1`–`h6` está errada. Erros típicos que o validador apanha:

| Mensagem | Causa |
|---|---|
| `A document must not include more than one visible "main" element.` | Dois `<main>` |
| `Element "p" not allowed as child of element "ul" in this context.` | `<p>` dentro de `<ul>` (só pode haver `<li>`) |
| `Stray start tag "td".` | `<td>` fora de `<tr>` |
| `A table row was 4 columns wide and exceeded the column count established by the first row (2).` | Linha com colunas a mais (aviso) |

## Git neste repositório

O repositório principal segue toda a pasta da UC, incluindo o material do docente.

A pasta `03_Trabalho_Pratico/Proj_Aulas/PL02_2022148GoncaloFernandes/` tem o seu próprio `.git`, com remoto em `https://github.com/ltarkker/PL02_2022148GoncaloFernandes.git`. Ao mesmo tempo, o `index.html` dessa pasta está seguido pelo repositório principal. Consequências:

- Alterações ao `index.html` da PL02 aparecem em dois repositórios e têm de ser commitadas em ambos.
- O `README.md` da PL02 pertence ao repositório interno; o principal vê-o como ficheiro não seguido.
- Para publicar a PL02 no GitHub: `git -C 03_Trabalho_Pratico/Proj_Aulas/PL02_2022148GoncaloFernandes push`.

Se o objectivo for ter apenas um histórico, as opções são remover o `.git` interno (e manter só o repositório principal) ou converter a pasta num submódulo. Qualquer das duas é uma decisão a tomar antes do TP01, quando o Git passa a ser útil para o trabalho.

Convenção de mensagens de commit usada até agora: `tipo(âmbito): descrição` (ex.: `chore(repo): initial commit`, `fix(repo): add missing extension`).
