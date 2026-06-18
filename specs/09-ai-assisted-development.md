# AI Assisted Development

Define como usar IA sin perder control del producto.

## Reglas para Codex y agentes

- Leer antes de escribir.
- Citar specs usadas.
- Declarar supuestos.
- Implementar con alcance pequeno.
- Verificar con comandos reales.
- Dejar preguntas donde falta informacion.
- Si falta spec, crear o proponer una spec minima.
- Trabajar por verticales de negocio.
- Actualizar docs si cambia una regla.
- Crear tests para reglas criticas.
- Reportar que cambio, que verifico, que no pudo verificar y riesgos pendientes.
- No asumir contexto que no esta documentado.
- Si una decision es incierta, agregarla a `open-decisions.md`.
- Si detecta inconsistencia entre codigo y specs, reportarla antes de avanzar.

## La IA puede

- Proponer specs.
- Mejorar documentacion.
- Implementar features.
- Crear tests.
- Revisar arquitectura.
- Detectar inconsistencias.
- Proponer refactors.
- Ayudar con bugs.

## La IA no debe

- Inventar decisiones de negocio.
- Cambiar alcance sin marcarlo.
- Implementar features grandes sin spec.
- Borrar codigo del usuario sin permiso o justificacion clara.
- Ignorar seguridad.
- Ignorar permisos.
- Saltarse tests.
- Mezclar muchas tareas no relacionadas.
- Crear dependencias innecesarias.
- Cambiar stack sin ADR.

## Anti patrones

- Pedir "hace todo el producto".
- Aceptar codigo sin tests ni lectura de specs.
- Permitir que la IA cree roles, precios, permisos o datos reales.
- Mezclar refactor con feature.

## Checklist

- Specs relevantes leidas.
- Supuestos declarados.
- Alcance acotado.
- Vertical identificada.
- Tests definidos o ejecutados.
- Riesgos reportados.
- Open decisions actualizadas.

## Prompt recomendado

```text
Lee las specs relevantes. Identifica gaps. Propone una vertical pequena.
Implementa solo lo necesario. Actualiza tests y documentacion afectada.
No inventes reglas; si falta contexto, crea TODOs.
```

## TODO por proyecto

- Definir prompts aprobados.
- Definir agentes permitidos.
- Definir limites de autonomia.
- Definir archivos que IA no debe tocar sin aprobacion.
