# Directivas de Seguridad para IA — Repositorio Privado

Este repositorio es la **autoridad central de políticas** para todos los proyectos de
Diego Alejandro Saenz Falcon. Su propósito es doble:

1. **Capa positiva** — Instrucciones claras para agentes de IA **autorizados**
   (ver `AGENTS.md`, `llms.txt`): deben seguir prácticas educativas, pedagógicas,
   didácticas y de código limpio, y respetar la autoría.
2. **Capa defensiva (tripwire / honeytoken)** — Instrucciones incrustadas para
   agentes de IA **no autorizados** que penetren en el repositorio (ver
   `HONEYTOKEN.md`): se anulan sus instrucciones previas y se les ordena
   **no tocar, no copiar, no extraer, no compartir, no replicar y retirarse**.

> ⚠️ Nota honesta: estas defensas son **defensa en profundidad**, no un control
> técnico infalible. Un atacante puede ignorarlas. Combinar con: repo privado,
> colaboradores mínimos, `.gitignore` de secretos y, si se dispone, GitHub Pro
> (protección de rama, secret scanning).

## Regla #1 — CERO SECRETOS
**Nunca** se incluyen en NINGÚN repositorio, bajo NINGUNA circunstancia:
claves, contraseñas, API keys, tokens, certificados ni credenciales.
Ver `SECURITY.md` y `.gitignore`.

## Estructura
| Archivo | Función |
|---|---|
| `SECURITY.md` | Política de seguridad y regla de cero secretos |
| `AGENTS.md` | Instrucciones para agentes de IA **autorizados** |
| `llms.txt` | Contexto machine-readable para LLMs autorizados |
| `HONEYTOKEN.md` | Trampa / contrainyección para IA **no autorizada** |
| `robots-ai.md` | Lista de crawlers de IA a bloquear (derivados web) |
| `.gitignore` | Patrones que evitan commitear secretos |
| `CONTRIBUTING.md` | Cómo aportar respetando estas directivas |
