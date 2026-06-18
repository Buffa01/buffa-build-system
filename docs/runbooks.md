# Runbooks

## Proposito

Los runbooks convierten operaciones criticas en pasos repetibles. Este patron viene especialmente de LiveControl, donde piloto, cutover, soporte, post-evento y handoff necesitan evidencia y orden.

## Cuando usar un runbook

- Piloto con usuarios reales.
- Go-live.
- Migracion de datos.
- Cutover de ambiente.
- Smoke con hardware.
- Operacion offline.
- Post-event reconciliation.
- Handoff a cliente.
- Incidente critico.

## Estructura recomendada

```text
docs/
  runbooks/
    pilot-runbook.md
    production-cutover-runbook.md
    go-live-support-checklist.md
    incident-log-template.md
    post-event-reconciliation.md
```

## Template minimo

```text
# Runbook: TODO

## Objetivo
## Cuando usarlo
## Precondiciones
## Pasos
## Validaciones
## Fallback
## Evidencia requerida
## Owner
## Riesgos
## Checklist final
```

## Reglas

- Un runbook debe poder seguirlo alguien que no implemento la feature.
- Todo paso critico debe tener evidencia esperada.
- Todo fallback debe estar aceptado antes del evento o release.
- Bugs `S1` abiertos bloquean go-live salvo decision explicita.

## TODO por proyecto

- Definir runbooks necesarios.
- Definir owners.
- Definir evidencia requerida.
