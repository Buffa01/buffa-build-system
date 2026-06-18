# AGENTS.md

Este archivo define como deben operar Codex y otros agentes IA dentro de un proyecto que adopta buffa-build-system.

## Principios

- Leer specs antes de editar codigo.
- Ejecutar cambios pequenos, verificables y alineados a una task.
- No inventar reglas de negocio.
- No modificar arquitectura sin ADR o aprobacion explicita.
- No mezclar verticales no relacionadas.
- Reportar gaps entre spec, codigo y tests.
- Usar `Explorer` para auditar antes de adaptar un proyecto existente.
- Usar `Documentator` para pasar decisiones de chat a specs/status.
- Usar `Planner` antes de implementar features grandes.
- Usar `Tester Reviewer` como revision con contexto fresco.

## Flujo obligatorio

1. Identificar la task o spec activa.
2. Leer reglas globales y modulo afectado.
3. Revisar arquitectura, permisos, data model y testing.
4. Implementar el cambio minimo que cumple la vertical.
5. Agregar o actualizar tests.
6. Ejecutar verificaciones disponibles.
7. Resumir cambios, riesgos y pendientes.

## Flujo para adaptar un proyecto existente

1. `Explorer`: leer estructura, docs, stack, modulos y riesgos.
2. `Documentator`: crear propuesta documental y matriz de adaptacion.
3. `Planner`: ordenar primera migracion o primera vertical.
4. `Implementer`: tocar codigo solo cuando haya spec/task.
5. `Tester Reviewer`: revisar contra specs y tests.

## Limites de agentes

Un agente puede:

- Proponer specs.
- Implementar codigo segun specs.
- Crear tests.
- Revisar drift.
- Documentar decisiones.

Un agente no puede:

- Cambiar objetivos de producto sin aprobacion.
- Usar credenciales reales.
- Introducir servicios pagos sin decision registrada.
- Saltar permisos, seguridad o tests criticos.
- Hacer refactors grandes sin task dedicada.

## Roles operativos

- `agents/explorer.md`: lectura y diagnostico sin editar.
- `agents/documentator.md`: documentacion, specs, status y decisiones.
- `agents/planner.md`: plan de implementacion por verticales.
- `agents/implementer.md`: implementacion acotada.
- `agents/tester-reviewer.md`: revision independiente.

## Ejemplo

```text
Antes de implementar la pantalla de ventas, lee specs/modules/sales/prd.md,
rules.md, permissions.md, data-model.md y test-plan.md. Si falta el flujo de
cierre de caja, no lo inventes: deja una pregunta en open-decisions.md.
```

## TODO por proyecto

- Agregar comandos reales de test y lint.
- Agregar rutas criticas del codigo.
- Agregar agentes permitidos en el equipo.
- Agregar restricciones de seguridad del dominio.
