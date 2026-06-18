# Status

## Proposito

`status/` permite retomar un proyecto sin depender del chat, memoria personal o contexto de una sesion anterior.

Este patron viene de OrderNow y debe usarse en proyectos donde Codex, agentes o humanos trabajen por sesiones.

## Cuando usarlo

- Al cerrar una jornada de trabajo.
- Cuando cambia la proxima vertical.
- Cuando se toma una decision importante.
- Cuando se actualizan specs o tasks.
- Cuando queda una pregunta abierta que afecta implementacion.

## Estructura recomendada

```text
status/
  README.md
  next.md
  daily/
    YYYY-MM-DD.md
```

## Reglas

- `next.md` debe decir que hacer al retomar.
- `daily/` debe registrar decisiones, docs, tasks, codigo y preguntas.
- El status no reemplaza specs ni ADRs.
- Si una decision cambia arquitectura, permisos, datos o seguridad, debe ir tambien a ADR u open decision.

## Checklist

- Estado actual claro.
- Ultimo trabajo completado claro.
- Proxima vertical definida.
- Comandos utiles documentados.
- Riesgos y preguntas abiertas visibles.

## TODO por proyecto

- Crear `status/next.md`.
- Crear primer daily status.
- Definir frecuencia de actualizacion.
