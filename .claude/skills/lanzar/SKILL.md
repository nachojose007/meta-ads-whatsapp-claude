---
name: lanzar
description: Arma en Meta una campaña o una tanda de anuncios nuevos con destino WhatsApp (objetivo Interacción, conversaciones), paso a paso y con confirmación, y verifica en vivo que haya quedado como se pidió. Usar con "/lanzar", "subamos estos videos", "armemos una campaña".
---

# Lanzar

1. Leé `NEGOCIO.md` y `criterio/02-estructura.md` y `criterio/03-creativos.md`.
2. Preguntá qué material hay (videos/fotos y dónde están) y si los anuncios van a la campaña
   principal o a una de testeo.
3. Armá la **propuesta por escrito** antes de crear nada:
   - Campaña: nombre, objetivo Interacción (`OUTCOME_ENGAGEMENT`), presupuesto diario a nivel
     campaña, fecha y hora de inicio.
   - Conjunto: destino WhatsApp, meta de rendimiento conversaciones (`CONVERSATIONS`),
     ubicación (radio o barrios, "personas que viven en"), edad amplia, ubicaciones automáticas,
     página y número de WhatsApp.
   - Anuncios: nombre, archivo, texto principal, título, botón "Enviar mensaje de WhatsApp",
     mensaje precargado.
   - Total de gasto diario nuevo que suma a la cuenta.
4. Esperá el "sí". Creá en este orden: campaña (pausada) → conjunto → creativos → anuncios.
5. Releé todo en vivo: estados, presupuesto, ubicación, destino WhatsApp, start_time. Mostrá
   la vista previa (`ads_get_ad_preview`) si se puede.
6. Recién con todo verificado, proponé activar. Activá con el "sí" y releé de nuevo.
7. Anotá en `bitacora.md` ids, presupuesto y cuándo se juzga (2-3 días).
