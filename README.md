# ViewState Docs

Documentação da marca e do design system do **ViewState**, construída com
[MkDocs](https://www.mkdocs.org/) e o tema
[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

📖 **Site:** <https://viewstate360.github.io/viewstate-docs/>

## Conteúdo

- **Marca** — logo, conceito, variações e paleta de cores
- **Design System** — tipografia, fundações, componentes, feedback, dados e navegação

## Rodando localmente

```bash
python -m venv .venv
source .venv/bin/activate     # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

Acesse <http://127.0.0.1:8000>.

## Comandos úteis

| Comando | O que faz |
| ------- | --------- |
| `mkdocs serve` | Servidor local com recarga automática |
| `mkdocs build --strict` | Gera o site em `site/` e falha em links quebrados |
| `mkdocs gh-deploy` | Publica manualmente na branch `gh-pages` |

## Publicação automática

Todo push na branch `main` dispara `.github/workflows/deploy.yml`, que publica
o site na branch `gh-pages`.

> Na primeira vez, habilite em
> **Settings → Pages → Build and deployment → Deploy from a branch → `gh-pages` / `root`**.

## Cores da marca

| Token | Hex |
| ----- | --- |
| Brand Ring | `#31424E` |
| Brand Door | `#4F8A86` |
