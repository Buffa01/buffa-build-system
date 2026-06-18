# Domain Strategy

Define como modelar el negocio sin que la IA lo simplifique de mas.

## Reglas

- Usar lenguaje del dominio.
- Nombrar entidades segun el negocio, no segun la UI.
- Documentar invariantes.
- Separar acciones del usuario de efectos del sistema.
- Evitar modelos genericos como `Item` o `Record` si el dominio tiene nombres reales.

## Invariantes

| Invariante | Motivo | Test requerido |
| --- | --- | --- |
| TODO | TODO | TODO |

## Ejemplo

```text
Una sale cerrada no puede cambiar sus items; solo puede anularse con auditoria.
```

## Eventos de dominio

- TODO: entidad creada.
- TODO: estado cambiado.
- TODO: accion auditada.

## TODO por proyecto

- Definir vocabulario.
- Definir invariantes.
- Definir estados validos.
- Definir eventos importantes.
