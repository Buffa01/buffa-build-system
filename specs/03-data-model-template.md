# Data Model Template

Define entidades, relaciones, ownership y reglas de persistencia.

## Entidades principales

| Entidad | Descripcion | Owner | Persistencia |
| --- | --- | --- | --- |
| TODO | TODO | TODO | TODO |

## Reglas

- Toda entidad debe tener propietario funcional.
- Toda relacion critica debe tener cardinalidad clara.
- Toda entidad sensible debe tener reglas de acceso.
- Todo cambio de schema debe incluir migracion y test.

## Ejemplo

```text
Event 1..N PointOfSale
PointOfSale 1..N Sale
Sale 1..N SaleItem
```

## Campos requeridos por entidad

- Identificador: TODO
- Timestamps: TODO
- Tenant/organization: TODO
- Estado: TODO
- Auditoria: TODO

## TODO por proyecto

- Completar entidades reales.
- Marcar datos sensibles.
- Definir claves unicas.
- Definir estrategia de migraciones.
