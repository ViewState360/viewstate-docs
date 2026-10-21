# Contribuindo

## Rodando localmente

```bash
python -m venv .venv
source .venv/bin/activate     # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

A documentação fica em <http://127.0.0.1:8000>.

## Estrutura

```text
viewstate-docs/
├── mkdocs.yml                  # configuração do site e navegação
├── requirements.txt
└── docs/
    ├── index.md
    ├── marca/                  # logo e cores
    ├── design-system/          # tipografia, fundações, componentes...
    ├── assets/
    │   ├── marca/              # logos, símbolo e favicon
    │   └── ui/                 # painéis do UI Foundation v0.1
    └── stylesheets/extra.css   # tokens de cor do tema
```

## Adicionando uma página

1. Crie o `.md` dentro de `docs/`.
2. Registre o caminho em `nav`, no `mkdocs.yml`.
3. Rode `mkdocs build --strict` para checar links quebrados.

## Mexendo nas cores do site

Os tokens ficam em [`docs/stylesheets/extra.css`](https://github.com/ViewState360/viewstate-docs/blob/main/docs/stylesheets/extra.css).
Ao mudar uma cor da marca, atualize também a página [Cores](marca/cores.md).

## Publicação

Todo push na `main` dispara o workflow `.github/workflows/deploy.yml`, que faz
o build e publica na branch `gh-pages`.
