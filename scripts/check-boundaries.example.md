# Script Example: Check Boundaries

## Objetivo

Evitar imports ilegales entre modulos.

## Regla sugerida

- UI no importa database directamente.
- Domain no importa framework web.
- Modulos no acceden a internos de otros modulos.

## Pseudocodigo

```text
load boundary rules
scan imports
fail on forbidden dependency
```

## TODO por proyecto

- Definir carpetas.
- Definir reglas de imports.
