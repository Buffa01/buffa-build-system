# Source Project Analysis

## Proposito

Este documento registra que patrones reales se tomaron de proyectos en desarrollo para construir buffa-build-system. Usarlo cuando se quiera revisar si la base representa la forma real de trabajo y no solo una teoria.

## Proyectos fuente analizados

| Proyecto | Tipo | Aportes principales |
| --- | --- | --- |
| LiveControl | POS/event operations, web + mobile + offline | Specs globales, specs por modulo, verticales de negocio, package boundaries, runbooks de piloto, mobile readiness, offline sync, RLS, auditoria |
| StayControl | SaaS multi-tenant para alojamientos | Monorepo por apps/packages, specs base limpias, agentes por rol tecnico, multi-tenancy desde dia uno, backend como fuente de reglas |
| OrderNow | Food ordering, mobile + web + API | `status/`, daily logs, roles Explorer/Documentator/Planner/Implementer/Tester Reviewer, vertical slices, continuidad de trabajo |
| FoodControl | iOS local-first nutrition app | Docs por product/architecture/features/data-models/business-rules/testing, feature spec template, localizacion, privacidad, testing de dominio, MVVM pragmatico |

## Patrones comunes que pasan a la base

- Spec-Driven Development antes de features importantes.
- Specs y docs versionadas en el repo.
- Separacion entre producto, arquitectura, datos, permisos, testing y agentes.
- Trabajo por verticales completas, no por capas aisladas.
- Dominio y backend como fuente de reglas criticas.
- Multi-tenancy y permisos definidos antes de datos reales cuando aplica.
- Boundaries entre apps, packages, dominio, infraestructura y UI.
- Checklists y runbooks para piloto, produccion y handoff.
- Estado operativo del proyecto para poder retomar sin depender del chat.
- Roles de agentes separados entre explorar, documentar, planificar, implementar y revisar.

## Mejoras agregadas sobre los proyectos fuente

- Unificar la estructura para que sirva a SaaS, POS, mobile, dashboard, marketplace e internal tools.
- Separar roles genericos de agentes tecnicos y roles operativos.
- Agregar `status/` como pieza obligatoria para continuidad.
- Agregar templates de scripts para checks automatizables.
- Agregar matriz de adaptacion para decidir que aplica, que se adapta y que no aplica.

## Regla

Cuando un nuevo proyecto demuestre un patron mejor que esta base, se debe registrar aqui antes de modificar la metodologia global.

## TODO por proyecto

- Agregar nuevos proyectos fuente.
- Registrar patrones que funcionaron.
- Registrar patrones descartados y motivo.
