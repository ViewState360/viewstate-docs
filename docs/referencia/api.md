# Referência da API

**URL base:** `https://exemplo.viewstate.app/v1`

## Autenticação

```bash
curl -H "Authorization: Bearer $TOKEN" \
  https://exemplo.viewstate.app/v1/health
```

## Endpoints

### `GET /health`

Verifica se o serviço está no ar.

**Resposta `200`**

```json
{
  "status": "ok"
}
```

### `GET /recurso`

> Documente parâmetros, corpo da requisição e respostas de cada endpoint.

**Parâmetros**

| Nome | Em | Tipo | Obrigatório | Descrição |
| ---- | -- | ---- | ----------- | --------- |
| —    | —  | —    | —           | —         |

## Códigos de erro

| Código | Significado |
| ------ | ----------- |
| `400`  | Requisição inválida |
| `401`  | Não autenticado |
| `403`  | Sem permissão |
| `404`  | Não encontrado |
| `500`  | Erro interno |
