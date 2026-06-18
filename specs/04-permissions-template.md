# Permissions Template

Define roles, permisos y reglas de acceso.

## Roles

| Rol | Descripcion | Puede | No puede |
| --- | --- | --- | --- |
| TODO | TODO | TODO | TODO |

## Reglas

- Deny by default.
- Cada accion sensible debe requerir permiso explicito.
- UI y backend deben validar permisos.
- Los permisos no deben depender solo de ocultar botones.
- Toda excepcion requiere decision documentada.

## Ejemplo

```text
cashier puede crear sales en su POS asignado.
cashier no puede editar precios ni ver reportes financieros globales.
admin puede configurar catalogo y usuarios.
```

## Matriz

| Accion | Owner | Admin | Operator | Readonly |
| --- | --- | --- | --- | --- |
| TODO | TODO | TODO | TODO | TODO |

## TODO por proyecto

- Definir roles reales.
- Definir permisos por modulo.
- Definir reglas multi-tenant.
- Definir auditoria de cambios.
