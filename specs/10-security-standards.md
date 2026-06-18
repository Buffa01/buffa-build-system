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

## Inputs

- Todo input externo debe validarse.
- Todo input del usuario debe sanitizarse cuando aplique.
- No confiar en datos del frontend.
- Validar tipos, rangos, formatos y permisos.
- Validar archivos subidos.
- Validar IDs recibidos por URL o body.
- Evitar SQL injection, NoSQL injection, command injection, XSS y path traversal.

## Auth y permisos

- Toda accion sensible requiere usuario autenticado.
- Toda accion sensible requiere permisos explicitos.
- No confiar solo en ocultar botones en UI.
- Backend/domain debe validar permisos.
- Las sesiones, tokens y cookies deben tener expiracion y configuracion segura.

## Multi-tenant

Si el proyecto es multi-tenant:

- Toda entidad operativa debe tener `tenantId`, `organizationId` o `businessId` segun corresponda.
- Nunca devolver datos de otro tenant.
- Las queries deben filtrar por tenant.
- Las policies/RLS deben definirse antes de usar datos reales.
- Los tests deben cubrir aislamiento entre tenants.

## Secrets

- No commitear secretos.
- No guardar tokens en codigo.
- Usar variables de entorno.
- Incluir `.env.example` cuando aplique.
- Nunca imprimir secretos en logs.

## Logs

- No loguear passwords, tokens, datos sensibles o informacion privada.
- Los logs deben ayudar a debuggear sin exponer datos innecesarios.
- Los errores externos deben registrarse con IDs o codigos, no con payloads sensibles completos.

## Rate limit

- Endpoints publicos o sensibles deben considerar rate limiting.
- Login, recovery, pagos, invitaciones y acciones criticas deben protegerse contra abuso.

## Ejemplo

```text
Un admin puede invitar usuarios, pero no puede leer tokens de sesion ni secrets.
```

## Checklist

- Inputs validados.
- Auth requerida.
- Permisos backend aplicados.
- Tenant isolation revisada.
- Secrets fuera del repo.
- Logs sin datos sensibles.
- Rate limits considerados.
- Errores no exponen informacion innecesaria.

## TODO por proyecto

- Definir datos sensibles.
- Definir threat model basico.
- Definir manejo de secrets.
- Definir auditoria.
