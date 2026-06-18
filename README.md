# buffa-build-system

Tambien puede usarse como:

- Buffa AI Development System
- Buffa Spec-Driven Development System
- Buffa Product Build System

Este repositorio no es un producto final. Es una fuente raiz reutilizable para crear, adaptar y gobernar productos digitales con IA, Codex y agentes de desarrollo bajo Spec-Driven Development.

## Filosofia

Specs definen la verdad. Agentes ejecutan con limites. Tasks convierten specs en verticales. Tests protegen reglas criticas. Scripts automatizan lo que no debe depender de prompts. Review evita drift entre documentacion y codigo.

## Para que sirve

Usa este repo como referencia al iniciar o revisar proyectos como LiveControl, StayControl, FoodControl, AgendaControl, ShopWise, SaaS, apps mobile, POS, dashboards, sistemas internos o productos digitales futuros.

Prompt base:

```text
Analiza este nuevo proyecto, entende su producto, stack, dominio y estado actual, y adapta el modelo de buffa-build-system a este proyecto.
```

## Estructura principal

- `specs/`: verdad del producto, arquitectura, dominio, seguridad, testing y reglas globales.
- `specs/modules/`: plantilla para documentar modulos funcionales.
- `agents/`: roles, limites y responsabilidades para agentes IA.
- `tasks/`: verticales de ejecucion orientadas a valor de negocio.
- `prompts/`: prompts reutilizables para Codex y agentes.
- `docs/`: onboarding, glosario y salud del proyecto.
- `adr/`: decisiones tecnicas persistentes.
- `checklists/`: controles antes de construir, revisar y lanzar.
- `scripts/`: automatizaciones sugeridas para evitar depender de prompts.
- `.github/`: plantillas de issues y pull requests.
- `AGENTS.md` y `CODEX.md`: reglas operativas para IA.

## Como usarlo en un proyecto nuevo

1. Copiar o referenciar este repo desde el proyecto real.
2. Completar `specs/00-product-vision-template.md`.
3. Adaptar `specs/01-global-rules.md`, `02-architecture-template.md` y `03-data-model-template.md`.
4. Crear un modulo en `specs/modules/<nombre-del-modulo>/`.
5. Convertir el modulo en verticales usando `tasks/vertical-template.md`.
6. Ejecutar con agentes siguiendo `AGENTS.md` y `CODEX.md`.
7. Agregar tests y scripts de verificacion antes de considerar terminada una vertical.
8. Registrar decisiones importantes en `adr/`.

## Regla central

La IA no debe inventar producto, datos, permisos, integraciones, arquitectura ni reglas de negocio. Si falta informacion, debe dejar una pregunta o un `TODO` explicito en la spec correspondiente.

## TODO por proyecto

- Definir nombre del producto.
- Definir usuarios, roles y permisos.
- Definir stack real.
- Definir modulos iniciales.
- Definir roadmap por verticales.
- Definir comandos reales de build, test, lint y deploy.
- Definir reglas de seguridad y datos sensibles.
