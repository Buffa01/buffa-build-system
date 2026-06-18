# Codex Local Configuration

## Proposito

Esta carpeta documenta como llevar los playbooks de agentes a configuraciones locales de Codex cuando el proyecto lo necesite.

El patron viene de OrderNow: los agentes viven versionados en `agents/` y pueden reflejarse en `.codex/agents/` para que sean portables entre maquinas o superficies de Codex.

## Regla

La fuente de verdad sigue siendo `agents/`. `.codex/` no debe contradecir esos playbooks.

## Estructura recomendada

```text
.codex/
  README.md
  agents/
    README.md
```

## Cuando usarlo

- Si el proyecto define agentes custom invocables por nombre.
- Si varias maquinas necesitan la misma configuracion local.
- Si el equipo quiere separar roles como explorer, documentator, planner, implementer y tester-reviewer.

## TODO por proyecto

- Definir si Codex custom agents aplica.
- Crear archivos concretos de agentes si el entorno los consume.
