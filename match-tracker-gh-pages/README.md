# Match Tracker — Futsal (GitHub Pages)

Este pacote está **pronto** para publicar no GitHub Pages.

## Estrutura
```
.
├─ index.html   ← a tua app (ficheiro original renomeado)
├─ 404.html     ← página de erro (opcional, mas recomendada)
└─ README.md
```

## Como publicar (opção A — raiz do repositório)
1. Cria um repositório no GitHub, por exemplo `match-tracker`.
2. Faz upload dos ficheiros `index.html` e `404.html` para a **branch `main`**, na raiz do repositório.
3. Em **Settings → Pages**:
   - *Source*: **Deploy from a branch**
   - *Branch*: **main** / **/** *(root)*
4. O teu site ficará disponível em `https://<o_teu_utilizador>.github.io/match-tracker/`.

## Como publicar (opção B — pasta `docs/`)
1. Cria uma pasta `docs` no repositório e coloca lá os ficheiros.
2. Em **Settings → Pages** escolhe **main** / **/docs**.

## Notas úteis
- **Sem dependências**: Tudo está num único `index.html` com CSS/JS embutido; nenhum build é necessário.
- **Armazenamento local**: Os dados (perfis, fotos, estatísticas) guardam-se em `localStorage` no teu navegador (chave: `match-tracker-v12`). Isto significa que:
  - Cada dispositivo/telemóvel tem o seu próprio estado.
  - Se precisares de “limpar” o estado, usa o botão **Reset** dentro da app ou limpa o `localStorage` do site.
- **Exportar CSV**: A função de exportação cria um ficheiro para download diretamente no navegador – funciona bem no GitHub Pages.
- **Fotos/avatares**: As imagens que adicionares ficam guardadas localmente (base64) no dispositivo; não são carregadas para o GitHub.

Bom jogo! ⚽