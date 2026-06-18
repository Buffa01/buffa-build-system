# CODEX.md

Guia operativa para usar Codex en proyectos basados en buffa-build-system.

## Modo de trabajo

Codex debe actuar como ingeniero de producto: entender specs, tocar codigo con alcance limitado, verificar y reportar drift.

## Orden de lectura recomendado

1. `README.md`
2. `specs/01-global-rules.md`
3. `specs/00-product-vision-template.md`
4. `specs/02-architecture-template.md`
5. `specs/modules/README.md`
6. Modulo especifico afectado
7. Task activa
8. `status/next.md` si existe

## Reglas para prompts

- Pedir siempre que Codex cite las specs usadas.
- Pedir que liste supuestos antes de implementar.
- Pedir que convierta features en verticales verificables.
- Pedir que no invente datos, APIs ni reglas.
- Pedir que deje TODOs en archivos correctos.

## Reglas obligatorias

- Antes de implementar, leer specs relevantes.
- Si falta spec, crear o proponer spec minima.
- Mantener cambios acotados.
- Trabajar por verticales de negocio.
- Actualizar docs si cambia una regla.
- Crear tests para reglas criticas.
- Reportar que cambio, que verifico, que no pudo verificar y riesgos pendientes.
- No asumir contexto no documentado.
- Si una decision es incierta, agregarla a `open-decisions.md`.
- Si detecta inconsistencia entre codigo y specs, reportarla antes de avanzar.

## Codex puede

- Proponer specs.
- Mejorar documentacion.
- Implementar features.
- Crear tests.
- Revisar arquitectura.
- Detectar inconsistencias.
- Proponer refactors.
- Ayudar con bugs.

## Codex no debe

- Inventar decisiones de negocio.
- Cambiar alcance sin marcarlo.
- Implementar features grandes sin spec.
- Borrar codigo del usuario sin permiso o justificacion clara.
- Ignorar seguridad o permisos.
- Saltarse tests.
- Mezclar muchas tareas no relacionadas.
- Crear dependencias innecesarias.
- Cambiar stack sin ADR.

## Ejemplo de instruccion

```text
Usa buffa-build-system. Lee specs, detecta el modulo afectado y crea una
vertical pequena. Implementa solo lo necesario, actualiza tests y reporta drift.
```

## Ejemplo para auditar proyecto existente

```text
Usa el rol Explorer. Analiza este proyecto sin editar archivos. Detecta stack,
estructura, modulos, docs, specs faltantes, riesgos y que partes de
buffa-build-system aplican tal cual, se adaptan o no aplican.
```

## TODO por proyecto

- Definir stack.
- Definir comandos locales.
- Definir convenciones de ramas.
- Definir estrategia de PR.
- Crear `status/next.md`.
