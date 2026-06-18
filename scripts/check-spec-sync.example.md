# Script Example: Check Spec Sync

## Objetivo

Detectar drift entre specs, tasks y codigo.

## Regla sugerida

- Si cambia un modulo core, revisar spec del modulo.
- Si cambia permisos, revisar permissions.
- Si cambia schema, revisar data model.

## Pseudocodigo

```text
map changed files to module
check expected spec files
warn or fail if missing
```

## TODO por proyecto

- Definir mapping codigo -> specs.
- Integrar con PR template.
