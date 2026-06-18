# Testing Strategy

Define como se protege el producto.

## Piramide practica

- Unit tests: reglas de dominio, validaciones y transformaciones.
- Integration tests: repositorios, APIs, auth, permisos y sincronizacion.
- E2E/smoke: flujos criticos del usuario.
- Manual QA: hardware, pagos, dispositivos o casos dificiles de automatizar.

## Reglas

- Toda regla critica debe tener test.
- Todo bug corregido debe dejar test o checklist.
- No confiar solo en snapshots visuales.
- Tests deben correr en CI cuando sea posible.

## Ejemplo

```text
Si un cashier no puede ver reportes financieros, debe existir test de API y UI.
```

## Criterios minimos

- Build pasa.
- Lint pasa.
- Tests criticos pasan.
- Smoke manual documentado si aplica.

## TODO por proyecto

- Definir framework de tests.
- Definir comandos.
- Definir cobertura minima por modulo.
- Definir casos no automatizables.
