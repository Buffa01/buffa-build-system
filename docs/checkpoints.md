# Checkpoints

## Proposito

Los checkpoints son revisiones documentales y tecnicas en momentos importantes. Este patron aparece en OrderNow y FoodControl para congelar estado, riesgos y siguiente paso.

## Tipos

- Project health checkpoint.
- Functional checkpoint.
- Backend/domain split checkpoint.
- Foundation review.
- API foundation review.
- Read-only foundation review.
- Production readiness checkpoint.

## Cuando crear uno

- Antes de una nueva fase.
- Despues de una vertical grande.
- Antes de migrar arquitectura.
- Antes de piloto o produccion.
- Cuando hay drift entre docs, codigo y tests.

## Template

```text
# Checkpoint - YYYY-MM-DD

## Contexto
## Estado actual
## Lo que esta solido
## Riesgos
## Drift detectado
## Tests y checks
## Decisiones tomadas
## Decisiones abiertas
## Proxima vertical recomendada
```

## TODO por proyecto

- Definir frecuencia de checkpoints.
- Definir quien los aprueba.
