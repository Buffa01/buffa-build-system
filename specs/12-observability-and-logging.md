# Observability and Logging

Define como entender el sistema en desarrollo y produccion.

## Logs

- Logs deben explicar eventos importantes.
- Logs no deben contener secretos.
- Errores deben incluir contexto tecnico suficiente.
- Acciones sensibles deben tener auditoria funcional.

## Metricas

- Disponibilidad: TODO
- Latencia: TODO
- Errores: TODO
- Negocio: TODO

## Alertas

- TODO: errores criticos.
- TODO: fallos de sincronizacion.
- TODO: fallos de pagos.
- TODO: degradacion de performance.

## Ejemplo

```text
sale_sync_failed debe incluir sale_id, pos_id, error_code y retry_count.
```

## TODO por proyecto

- Definir proveedor de logs.
- Definir eventos criticos.
- Definir dashboard operativo.
- Definir retencion de logs.
