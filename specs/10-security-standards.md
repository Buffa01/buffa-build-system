# Security Standards

Define reglas base de seguridad.

## Principios

- Deny by default.
- Least privilege.
- Secrets fuera del repo.
- Auditoria para acciones sensibles.
- Validacion en backend, no solo UI.
- Datos sensibles minimizados.

## Reglas

- No commitear `.env` reales, tokens, llaves privadas ni dumps.
- No loguear passwords, tokens, PII o datos financieros sensibles.
- Toda API sensible debe verificar auth y permisos.
- Toda operacion destructiva debe ser auditable.

## Ejemplo

```text
Un admin puede invitar usuarios, pero no puede leer tokens de sesion ni secrets.
```

## TODO por proyecto

- Definir datos sensibles.
- Definir threat model basico.
- Definir manejo de secrets.
- Definir auditoria.
