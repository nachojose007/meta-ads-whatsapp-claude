---
name: lectura
description: Tablero del día de Meta Ads para un negocio que vende por WhatsApp - gasto, conversaciones, costo por conversación y por cliente en ventanas de 4 y 7 días, contra la vara de NEGOCIO.md. Solo lectura. Usar con "/lectura", "cómo vamos", "cómo están los anuncios".
---

# Lectura del día

Solo lectura. No propone apagados (eso es `/optimizar`) salvo una alarma clara.

1. `date` para la fecha. Leé `NEGOCIO.md` (la vara) y las últimas líneas de `bitacora.md`.
2. Traé de la cuenta, a nivel cuenta y por campaña: ayer, últimos 4 días cerrados y últimos 7:
   gasto, conversaciones con mensajes iniciadas, costo por conversación, frecuencia, CTR saliente.
3. Si hay `registro/conversaciones.csv` con datos de esas fechas, sumá clientes y costo por
   cliente.
4. Entregá:
   - **Una línea de titular**: "Ayer: $X gastados, N conversaciones a $Y (vara $Z) 🟢/🟡/🔴".
   - Tabla por campaña con 4d y 7d.
   - Top 3 anuncios y los 3 peores de 4d (por `ad_id`).
   - Alarmas: campaña que no gastó, anuncio rechazado, costo 2x la vara, método de pago con error.
   - Qué mirar mañana.
5. Semáforo: 🟢 ≤ vara · 🟡 hasta 1,5 varas · 🔴 más de 1,5 varas o 0 conversaciones con gasto.
