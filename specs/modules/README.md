# Modules

Un modulo representa una capacidad funcional del producto.

Ejemplos:

- Sales
- Inventory
- Auth
- Reporting
- Billing
- Notifications
- Devices
- Catalog

## Como crear un modulo

1. Copiar `module-template/`.
2. Renombrar la carpeta.
3. Completar PRD, reglas, flows, permisos, API, data model y test plan.
4. Registrar decisiones abiertas.
5. Crear verticales en `tasks/`.

## Reglas

- Un modulo debe tener owner funcional.
- Un modulo debe declarar sus boundaries.
- Un modulo no debe depender de detalles internos de otro modulo.
- Toda integracion entre modulos debe tener contrato.

## TODO por proyecto

- Listar modulos reales.
- Marcar modulos core.
- Marcar modulos futuros.
