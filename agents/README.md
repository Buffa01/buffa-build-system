# Agents

Define roles especializados para IA. Un agente no es una persona: es un modo de trabajo con limites.

## Reglas generales

- Todo agente debe leer specs.
- Todo agente debe declarar alcance.
- Todo agente debe reportar gaps.
- Todo agente debe evitar cambios fuera de su rol.

## Agentes disponibles

- Explorer
- Documentator
- Planner
- Implementer
- Tester Reviewer
- Spec Writer
- Product
- Backend
- Frontend
- Mobile
- Database
- Testing
- Review
- Security
- DevOps
- Refactor

## TODO por proyecto

- Definir agentes habilitados.
- Definir owners humanos.
- Definir permisos de ejecucion.

## Orden recomendado

Para adaptar un repo existente:

```text
explorer -> documentator -> planner -> implementer -> tester-reviewer
```

Para crear una feature desde cero:

```text
spec-writer -> planner -> backend/frontend/mobile/database -> testing -> review/security
```
