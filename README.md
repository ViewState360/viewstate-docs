# ViewState Docs

Documentação do ViewState, construída com [MkDocs](https://www.mkdocs.org/) e o
tema [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

📖 **Site publicado:** <https://viewstate360.github.io/viewstate-docs/>

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

Todo push na branch `main` dispara o workflow `.github/workflows/deploy.yml`,
que faz o build e publica o site na branch `gh-pages`.

> Na primeira vez, habilite o GitHub Pages em
> **Settings → Pages → Build and deployment → Deploy from a branch → `gh-pages` / `root`**.

## Estrutura

```text
viewstate-docs/
├── mkdocs.yml          # configuração do site e navegação
├── requirements.txt    # dependências
└── docs/               # conteúdo em Markdown
```

Para contribuir, veja [docs/contribuindo.md](docs/contribuindo.md).
