# Script Example: Check File Size

## Objetivo

Evitar archivos demasiado grandes que dificultan review y trabajo con IA.

## Regla sugerida

- Avisar sobre archivos de codigo con mas de 300 lineas.
- Bloquear archivos con mas de 600 lineas salvo excepcion.

## Pseudocodigo

```text
for each source file:
  count lines
  warn if > 300
  fail if > 600
```

## TODO por proyecto

- Definir extensiones.
- Definir limites.
- Definir excepciones.
