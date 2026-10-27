# Meta Ads → WhatsApp, manejado con Claude Code

Un kit para que el dueño de un negocio local (estudio de yoga, consultorio, gimnasio,
peluquería, inmobiliaria) maneje sus anuncios de Meta desde Claude Code, con un objetivo:
**que lleguen conversaciones a WhatsApp que terminen en clientes**.

No es para tiendas online ni campañas de ventas con píxel. Es para negocios donde la venta
se cierra charlando.

📘 **Manual paso a paso (desde cero):** _ver el link que te pasaron junto con este repo_

## Qué trae

| Archivo | Qué es |
|---|---|
| `CLAUDE.md` | El cerebro: reglas, cómo piensa y qué nunca hace sin tu OK |
| `NEGOCIO.md` | La ficha de tu negocio (la completás con Claude en `/arranque`) |
| `criterio/` | El criterio de Meta: economía del mensaje, estructura, creativos, cuándo apagar, WhatsApp, trampas de la API |
| `.claude/skills/` | Los comandos: `/arranque`, `/lectura`, `/optimizar`, `/lanzar`, `/creativos`, `/registrar` |
| `registro/conversaciones.csv` | Dónde se anota qué conversaciones se volvieron clientes |
| `bitacora.md` | Qué se hizo, cuándo y por qué |

## Instalación rápida

1. Tener **Claude Code** instalado (app de escritorio de Claude, pestaña **Code**) con un plan Pro o Max.
2. Conectar **Meta Ads** en claude.ai → Configuración → Conectores.
3. Bajar este repo:
   - **Sin saber nada de Git:** botón verde **Code → Download ZIP**, descomprimir en Documentos.
   - **Con Git:** `git clone https://github.com/nachojose007/meta-ads-whatsapp-claude.git`
4. En Claude Code, abrir la carpeta `meta-ads-whatsapp-claude` y escribir:

```
/arranque
```

Claude te va a hacer unas preguntas sobre tu negocio, va a leer tu cuenta de Meta y te va a
dar un diagnóstico con los próximos pasos.

## El día a día

| Cuándo | Qué escribís |
|---|---|
| Cada mañana | `/lectura` |
| 2-3 veces por semana | `/optimizar` |
| Cada noche (2 minutos) | `/registrar` y le contás cuántos escribieron y cuántos se anotaron |
| Cuando tenés videos nuevos | `/lanzar` |
| Una vez por semana | `/creativos` para saber qué grabar |

También le podés hablar normal: "¿cómo vienen los anuncios esta semana?", "¿cuál video trae
más alumnos?", "bajemos el presupuesto a la mitad hasta el lunes".

## Seguridad

- Claude **lee libremente** pero **no cambia nada en Meta sin tu "sí"** con el monto escrito.
- Nunca toca medios de pago ni permisos.
- Nunca le escribe a un cliente sin que apruebes el texto.
- Tus datos (`NEGOCIO.md`, `registro/`, `bitacora.md`) quedan en tu computadora. **No los subas
  a un repo público.** Si querés versionarlos, hacé una copia privada del repo.

## Créditos

Criterio armado a partir de cómo manejamos Meta Ads con Claude Code en un e-commerce argentino
que invierte todos los días, adaptado a campañas de mensajes.
