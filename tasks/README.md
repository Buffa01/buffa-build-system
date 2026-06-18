# Tasks

Las tasks convierten specs en trabajo ejecutable.

## Proposito

Evitar que el trabajo se organice solo por capas tecnicas. Una task debe mover el producto hacia un flujo usable, verificable y conectado con specs.

## Cuando usarlo

- Para planificar una feature.
- Para dividir roadmap en entregables.
- Para pedir implementacion a Codex.
- Para revisar si una vertical esta realmente terminada.

## Reglas

- Una task debe tener objetivo, alcance y criterio de aceptacion.
- Una task debe nombrar specs afectadas.
- Una task debe terminar con verificacion.
- Una task no debe mezclar producto, refactor y hardening salvo que sea explicito.

## Ejemplo incorrecto

```text
1. Crear todas las tablas.
2. Crear todo el backend.
3. Crear todo el frontend.
4. Testear al final.
```

## Ejemplo correcto

```text
Vertical 1:
- Auth minima.
- Modelo necesario.
- Endpoint necesario.
- UI minima.
- Tests minimos.
- Flujo usable.

Vertical 2:
- Siguiente flujo de negocio completo.
- Datos reales.
- Validaciones.
- Permisos.
- Tests.
```

## Estructura recomendada

Cada vertical debe tener:

- Objetivo.
- Alcance.
- Specs relacionadas.
- Archivos esperados.
- Backend.
- Frontend/Mobile.
- Data model.
- Permisos.
- Tests.
- Criterios de aceptacion.
- Riesgos.
- Checklist de cierre.

## Tipos

- Setup
- Foundation
- Core flow
- Real data
- Dashboard/reports
- Hardening
- Pilot readiness
- Production readiness

## TODO por proyecto

- Crear backlog inicial.
- Marcar primera vertical.

## Checklist

- Task vinculada a spec.
- Resultado de negocio claro.
- Alcance y fuera de alcance definidos.
- Tests definidos.
- Riesgos definidos.
- Cierre verificable.
