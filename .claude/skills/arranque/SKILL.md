---
name: arranque
description: Primera vez con la cuenta. Completa NEGOCIO.md con el dueño, verifica que el MCP de Meta esté conectado, lee la cuenta y arma el diagnóstico inicial con la propuesta de estructura. Usar cuando el dueño dice "arrancamos", "/arranque" o NEGOCIO.md está vacío.
---

# Arranque

1. **Conexión.** Llamá a `ads_get_ad_accounts`. Si la herramienta no existe, el MCP de Meta no
   está conectado: explicale al dueño cómo conectarlo (README, paso "Conectar Meta") y pará acá.
   Si hay varias cuentas, preguntale cuál es la del negocio.
2. **Ficha.** Hacé las preguntas de `NEGOCIO.md` de a tandas cortas (máximo 4 por mensaje), en
   lenguaje simple. Empezá por los ⭐. Si no sabe un número, proponé un estimado razonable,
   marcalo "(estimado)" y seguí. Guardá las respuestas en `NEGOCIO.md`.
3. **La vara.** Calculá y mostrale: costo máximo por cliente y costo máximo por conversación.
   Pedile que lo valide.
4. **Lectura de la cuenta** (solo lectura): campañas activas y pausadas recientes, objetivo,
   presupuesto, ubicación del conjunto, y por anuncio los últimos 7 y 4 días de gasto,
   conversaciones iniciadas, costo por conversación, frecuencia. Cruzá por post_id.
   Verificá que haya un número de WhatsApp conectado a la página (`ads_get_ad_account_pages`).
5. **Diagnóstico** (corto, en este orden):
   - Cuánto se gasta por día y cuánto cuesta hoy una conversación contra la vara.
   - Estructura actual vs. la de `criterio/02-estructura.md` (¿hay que unificar?).
   - Los 3 anuncios que mejor andan y los que se llevan plata sin traer nada.
   - Cómo está el WhatsApp (mensaje de bienvenida, tiempo de respuesta) según lo que contó.
   - Propuesta de los próximos 7 días, numerada, con lo que necesita su "sí".
6. Anotá en `bitacora.md` la fecha del arranque y la vara acordada.
