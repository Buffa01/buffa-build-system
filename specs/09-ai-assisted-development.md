# AI Assisted Development

Define como usar IA sin perder control del producto.

## Reglas para Codex y agentes

- Leer antes de escribir.
- Citar specs usadas.
- Declarar supuestos.
- Implementar con alcance pequeno.
- Verificar con comandos reales.
- Dejar preguntas donde falta informacion.

## Anti patrones

- Pedir "hace todo el producto".
- Aceptar codigo sin tests ni lectura de specs.
- Permitir que la IA cree roles, precios, permisos o datos reales.
- Mezclar refactor con feature.

## Prompt recomendado

```text
Lee las specs relevantes. Identifica gaps. Propone una vertical pequena.
Implementa solo lo necesario. Actualiza tests y documentacion afectada.
No inventes reglas; si falta contexto, crea TODOs.
```

## TODO por proyecto

- Definir prompts aprobados.
- Definir agentes permitidos.
- Definir limites de autonomia.
- Definir archivos que IA no debe tocar sin aprobacion.
