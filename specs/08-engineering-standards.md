# Engineering Standards

Define calidad tecnica minima. Usar este archivo cuando Codex, agentes o humanos implementan codigo, revisan PRs o deciden si un refactor es necesario.

## Clean Architecture

El codigo debe separar responsabilidades:

- Domain: reglas de negocio, invariantes y entidades.
- Application / Use Cases: orquestacion de acciones del usuario o sistema.
- Infrastructure: adaptadores tecnicos, servicios externos y framework glue.
- UI / Presentation: pantallas, componentes, view state e interaccion.
- Data Access: queries, repositorios, storage, ORM y migraciones.
- Integrations: APIs externas, pagos, email, hardware, proveedores.

Reglas:

- La UI no debe contener reglas criticas de negocio.
- El dominio no debe depender de frameworks externos.
- Las validaciones criticas deben vivir en backend/domain, no solo en frontend.
- Los casos de uso deben ser pequenos, testeables y claros.
- Las integraciones externas deben estar encapsuladas.
- No mezclar logica de negocio con componentes visuales.
- No mezclar acceso a base de datos con reglas de UI.
- No duplicar reglas criticas en multiples lugares sin fuente de verdad.

## Codigo

- Preferir claridad sobre abstracciones prematuras.
- Mantener funciones pequenas y testeables.
- No duplicar reglas criticas.
- No mezclar UI, permisos y persistencia en el mismo lugar.
- No introducir dependencias sin necesidad clara.
- No dejar codigo muerto.
- No dejar `console.log`, debug prints o trazas innecesarias.
- No dejar TODOs criticos sin issue, ADR u open decision.
- No hacer refactors grandes dentro de features sin justificar.
- No cambiar formato masivamente si no es necesario.
- No borrar codigo del usuario sin explicar por que.

## Limites de archivos

Limites recomendados por defecto:

- Archivos de codigo: maximo recomendado 200 lineas.
- Componentes UI: maximo recomendado 150 lineas.
- Funciones: maximo recomendado 40 lineas.
- ViewModels / Controllers: maximo recomendado 200 lineas.
- Tests: pueden ser mas largos si estan bien organizados.

Excepciones permitidas solo si estan justificadas en comentario, issue o ADR. Si un archivo supera el limite, Codex debe proponer una division antes de seguir agregando logica.

## Naming

- Usar nombres claros y descriptivos.
- No usar nombres genericos como `data`, `item`, `thing` o `manager` sin contexto.
- No usar abreviaciones innecesarias.
- Los nombres deben expresar intencion de negocio.

Ejemplo:

```text
Incorrecto: processData(item)
Correcto: closeCashRegisterForPointOfSale(cashClose)
```

## Modularidad

- Cada modulo debe tener responsabilidad clara.
- Evitar dependencias circulares.
- Evitar modulos gigantes.
- Cada modulo con reglas importantes debe tener specs propias.
- Cada modulo debe declarar boundaries, contratos y datos que posee.

## Estructura

- Modulos con boundaries claros.
- Contratos explicitos.
- Tipos o schemas para datos de entrada y salida.
- Errores representables y manejables.

## Review

- Revisar behavior, no solo estilo.
- Buscar drift con specs.
- Buscar permisos faltantes.
- Buscar tests ausentes.
- Buscar archivos o funciones gigantes.
- Buscar dependencias innecesarias.
- Buscar mezcla de capas.

## Checklist

- La feature tiene spec minima.
- La logica critica no vive solo en UI.
- Los casos de uso son pequenos y testeables.
- Las integraciones estan encapsuladas.
- No hay cambios masivos de formato.
- No hay dependencias nuevas sin motivo.
- No hay archivos grandes sin plan de division.

## TODO por proyecto

- Definir formatter.
- Definir linter.
- Definir convenciones de carpetas.
- Definir reglas de imports.
