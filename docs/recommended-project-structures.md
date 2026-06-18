# Recommended Project Structures

## Proposito

Definir estructuras base reutilizables segun tipo de producto. Estas estructuras salen de patrones reales de LiveControl, StayControl, OrderNow y FoodControl.

## SaaS multi-tenant web

Inspirado en StayControl.

```text
apps/
  public-web/
  admin-panel/
  user-portal/
  api/
packages/
  database/
  domain/
  auth/
  permissions/
  validations/
  ui/
  config/
  testing/
  integrations/
specs/
tasks/
agents/
status/
```

Reglas:

- Backend como fuente de reglas.
- Toda entidad operativa con tenant.
- Apps no deben saltarse permisos ni acceder a datos de otro tenant.

## POS/event operations offline-tolerant

Inspirado en LiveControl.

```text
apps/
  web/
  cashier-mobile/
  hardware-bridge/
packages/
  domain/
  cashier-core/
  sync/
  printing/
  permissions/
  validations/
  testing/
specs/
  product/
  functional/
  technical/
  contracts/
  modules/
docs/
  runbooks/
tasks/
status/
```

Reglas:

- El flujo operativo principal no debe depender de internet si el negocio exige continuidad.
- Sync, printing y device context deben tener contratos.
- Runbooks de piloto y post-evento son parte del producto.

## Mobile local-first

Inspirado en FoodControl.

```text
App/
Core/
  Domain/
    Entities/
    ValueObjects/
    UseCases/
    Calculators/
  Data/
    Repositories/
    Mappers/
    Migrations/
  Services/
Features/
DesignSystem/
Resources/
Tests/
docs/
  product/
  architecture/
  features/
  data-models/
  business-rules/
  testing/
```

Reglas:

- Features no dependen directamente de persistencia.
- Dominio debe poder testearse sin UI, red ni base real.
- Localizacion, privacidad y estados UI deben estar en la spec de feature.

## Mobile + web + API ordering product

Inspirado en OrderNow.

```text
apps/
  mobile/
  web/
  api/
packages/
  shared/
  config/
docs/
specs/
tasks/
status/
agents/
.codex/
  agents/
```

Reglas:

- Separar app de usuario, panel operativo y API.
- Mantener `status/next.md` para retomar contexto.
- Usar agentes operativos para explorar, documentar, planificar, implementar y revisar.

## TODO por proyecto

- Elegir estructura objetivo.
- Marcar carpetas que ya existen.
- Marcar carpetas que se deben crear.
- Registrar excepciones.
