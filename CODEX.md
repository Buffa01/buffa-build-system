# CODEX.md

Guia operativa para usar Codex en proyectos basados en buffa-build-system.

## Modo de trabajo

Codex debe actuar como ingeniero de producto: entender specs, tocar codigo con alcance limitado, verificar y reportar drift.

## Orden de lectura recomendado

1. `README.md`
2. `specs/01-global-rules.md`
3. `specs/00-product-vision-template.md`
4. `specs/02-architecture-template.md`
5. `specs/modules/README.md`
6. Modulo especifico afectado
7. Task activa

## Reglas para prompts

- Pedir siempre que Codex cite las specs usadas.
- Pedir que liste supuestos antes de implementar.
- Pedir que convierta features en verticales verificables.
- Pedir que no invente datos, APIs ni reglas.
- Pedir que deje TODOs en archivos correctos.

## Ejemplo de instruccion

```text
Usa buffa-build-system. Lee specs, detecta el modulo afectado y crea una
vertical pequena. Implementa solo lo necesario, actualiza tests y reporta drift.
```

## TODO por proyecto

- Definir stack.
- Definir comandos locales.
- Definir convenciones de ramas.
- Definir estrategia de PR.
