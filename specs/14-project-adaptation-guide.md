# Project Adaptation Guide

Guia para adaptar buffa-build-system a un proyecto nuevo o existente.

## Paso 1: Entender el proyecto

- Producto.
- Usuarios.
- Stack.
- Estado actual.
- Modulos existentes.
- Riesgos.

Clasificar el tipo de producto:

- SaaS.
- POS.
- Mobile app.
- Marketplace.
- Dashboard.
- Landing.
- Internal tool.
- API.
- E-commerce.
- Sistema multi-tenant.

Identificar stack:

- Frontend.
- Backend.
- Mobile.
- Database.
- Auth.
- Infra.
- Testing.
- CI/CD.

Identificar madurez:

- Idea.
- MVP.
- Prototipo.
- Piloto.
- Produccion.
- Producto con usuarios.

## Paso 2: Mapear specs

- Completar vision.
- Completar arquitectura.
- Completar data model.
- Completar permisos.
- Completar roadmap.

## Paso 3: Crear modulos

Por cada area funcional importante, crear una carpeta basada en `specs/modules/module-template/`.

## Paso 4: Crear verticales

Usar `tasks/vertical-template.md` para convertir specs en entregables.

## Paso 5: Verificar drift

Comparar:

- Specs vs codigo.
- Codigo vs tests.
- Tasks vs roadmap.
- Permisos documentados vs permisos implementados.

## Tabla de adaptacion

Antes de tocar codigo, Codex debe generar una propuesta con esta tabla:

| Archivo base | Se usa tal cual | Se adapta | No aplica | Motivo | Prioridad |
| --- | --- | --- | --- | --- | --- |
| TODO | TODO | TODO | TODO | TODO | TODO |

Debe indicar:

- Que specs faltan.
- Que archivos de buffa-build-system aplicar tal cual.
- Que archivos adaptar.
- Que archivos no aplican.
- Que decisiones quedan abiertas.
- Que riesgos existen.
- Que orden de implementacion seguir.

## Regla

Codex debe generar primero una propuesta antes de tocar codigo. No debe borrar nada, no debe reestructurar masivamente y no debe cambiar codigo durante la fase de adaptacion documental.

## Prompt de adaptacion

```text
Analiza este proyecto existente. Usa buffa-build-system como modelo.
Detecta producto, stack, modulos, gaps y riesgos. Propone una adaptacion
incremental sin reescribir todo.
```

## TODO por proyecto

- Completar inventario inicial.
- Crear primera version de specs.
- Priorizar gaps.
- Definir primera vertical.
