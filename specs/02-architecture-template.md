# Architecture Template

Describe como esta construido el sistema y donde viven las responsabilidades.

## Stack

- Frontend: TODO
- Backend: TODO
- Mobile: TODO
- Database: TODO
- Auth: TODO
- Hosting: TODO
- Observability: TODO

## Principios

- Separar dominio, infraestructura y UI.
- Evitar dependencias circulares.
- Mantener contratos explicitos entre modulos.
- Preferir verticales pequenas sobre capas perfectas sin producto.

## Diagrama logico

```text
User -> UI -> Application Services -> Domain -> Persistence/External APIs
```

## Boundaries

| Area | Responsabilidad | No debe hacer |
| --- | --- | --- |
| UI | Presentar estado y capturar acciones | Reglas criticas de negocio |
| Domain | Reglas del producto | Llamar APIs externas directamente |
| Data | Persistencia y queries | Decidir permisos |
| Integrations | Servicios externos | Mutar dominio sin contrato |

## Decisiones pendientes

- TODO: monolito, modular monolith, microservicios u otro.
- TODO: estrategia offline.
- TODO: estrategia multi-tenant.

## TODO por proyecto

- Agregar diagrama real.
- Agregar carpetas reales.
- Agregar dependencias principales.
- Agregar tradeoffs aceptados.
