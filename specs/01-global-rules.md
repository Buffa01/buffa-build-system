# Global Rules

Estas reglas aplican a todo proyecto que adopte buffa-build-system.

## Reglas de verdad

- Las specs son la fuente de verdad.
- Ninguna feature importante debe implementarse sin una spec minima.
- El codigo implementa specs, no ideas sueltas.
- Las tasks traducen specs en verticales ejecutables.
- Los tests protegen reglas criticas.
- Los ADR documentan decisiones que cambian arquitectura, datos, seguridad o costos.

## Reglas para IA

- No inventar dominios, entidades, permisos, endpoints, integraciones ni flujos.
- Si falta contexto, registrar una pregunta en `open-decisions.md`.
- No optimizar antes de tener una vertical funcionando.
- No hacer cambios globales desde una task local.
- No borrar documentacion porque parezca vieja sin revisar codigo.

## Reglas de implementacion

- Cada vertical debe ser usable o verificable.
- Cada cambio debe tener criterio de aceptacion.
- Cada permiso debe estar definido antes de implementarse.
- Cada modelo de datos debe tener propietario y reglas de acceso.

## Ejemplo correcto

```text
La spec dice que cashier puede crear sales offline. La task implementa captura
local, persistencia local, sincronizacion y test de cola offline.
```

## Ejemplo incorrecto

```text
Agregar dashboard financiero porque parece util, aunque no existe en roadmap ni spec.
```

## TODO por proyecto

- Agregar reglas no negociables del negocio.
- Agregar restricciones tecnicas del stack.
- Agregar reglas de privacidad y compliance.
