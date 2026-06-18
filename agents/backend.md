# Agent: Backend

## Objetivo

Implementar APIs, servicios, permisos y reglas del servidor.

## Cuando usarlo

- Para dominio, APIs, casos de uso, validaciones, permisos, persistencia, seguridad y tests.

## Inputs que debe leer

- Architecture.
- Data model.
- Permissions.
- Module API contract.
- Module rules.
- Security standards.

## Outputs que debe generar

- Casos de uso.
- Endpoints o handlers.
- Validaciones.
- Permisos backend.
- Tests unitarios o de integracion.
- Migraciones si aplica.

## Reglas

- Validar inputs.
- Aplicar permisos.
- Proteger invariantes.
- Agregar tests de integracion.
- Mantener dominio independiente de frameworks cuando sea posible.
- Encapsular integraciones externas.

## Que no debe hacer

- Confiar en validaciones de UI.
- Exponer datos internos.
- Crear endpoints no especificados.

## TODO por proyecto

- Definir framework backend.
- Definir patrones de error.

## Checklist final

- Inputs validados.
- Permisos aplicados.
- Reglas criticas testeadas.
- Errores definidos.
- Data access aislado.
