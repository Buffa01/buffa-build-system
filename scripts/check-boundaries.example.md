# Script Example: Check Boundaries

## Objetivo

Evitar imports ilegales entre modulos.

## Regla sugerida

- UI no importa database directamente.
- Domain no importa UI.
- Domain no importa frameworks externos.
- Domain no importa framework web.
- UI no accede directo a DB.
- No imports circulares.
- Modulos no acceden a internos de otros modulos.
- Modulos no cruzan boundaries prohibidos.

## Pseudocodigo

```text
load boundary rules
scan imports
fail on forbidden dependency
```

## TODO por proyecto

- Definir carpetas.
- Definir reglas de imports.
