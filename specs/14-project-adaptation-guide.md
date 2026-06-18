# Project Adaptation Guide

Guia para adaptar buffa-build-system a un proyecto nuevo o existente.

## Paso 1: Entender el proyecto

- Producto.
- Usuarios.
- Stack.
- Estado actual.
- Modulos existentes.
- Riesgos.

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
