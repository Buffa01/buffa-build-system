# Script Example: Check File Size

## Objetivo

Evitar archivos demasiado grandes que dificultan review y trabajo con IA.

## Regla sugerida

- Avisar sobre archivos de codigo con mas de 200 lineas.
- Avisar sobre componentes UI con mas de 150 lineas.
- Avisar sobre funciones demasiado largas, por ejemplo mas de 40 lineas.
- Permitir tests mas largos si estan bien organizados.
- Permitir excepciones solo con comentario, issue o ADR.

## Pseudocodigo

```text
for each source file:
  count lines
  warn if code file > 200
  warn if UI component > 150
  detect functions > 40
  allow exception only if documented
```

## TODO por proyecto

- Definir extensiones.
- Definir limites.
- Definir excepciones.
