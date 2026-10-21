# Contribuindo

## Rodando a documentação localmente

```bash
# 1. Crie um ambiente virtual (opcional, mas recomendado)
python -m venv .venv
source .venv/bin/activate     # Windows: .venv\Scripts\activate

# 2. Instale as dependências
pip install -r requirements.txt

# 3. Suba o servidor local com recarga automática
mkdocs serve
```

A documentação fica disponível em <http://127.0.0.1:8000>.

## Estrutura do projeto

```text
viewstate-docs/
├── mkdocs.yml          # configuração do site e navegação
├── requirements.txt    # dependências da documentação
└── docs/
    ├── index.md
    ├── comecando/
    ├── guias/
    └── referencia/
```

## Adicionando uma página

1. Crie o arquivo `.md` dentro de `docs/`.
2. Registre o caminho na seção `nav` do `mkdocs.yml`.
3. Rode `mkdocs build --strict` para checar links quebrados.

## Publicação

Todo push na branch `main` dispara o workflow
[`.github/workflows/deploy.yml`](https://github.com/ViewState360/viewstate-docs/blob/main/.github/workflows/deploy.yml),
que publica o site na branch `gh-pages`.
