# Script Example: Check Secrets

## Objetivo

Evitar secrets commiteados.

## Buscar

- API keys.
- Tokens.
- Private keys.
- Passwords.
- `.env` reales.

## Pseudocodigo

```text
scan changed files
match secret patterns
fail with redacted output
```

## TODO por proyecto

- Integrar secret scanner real.
- Definir falsos positivos permitidos.
