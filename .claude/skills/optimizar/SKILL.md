---
name: optimizar
description: Propone qué anuncios apagar, cuáles dejar y qué escalar en Meta Ads, con el criterio de criterio/04-optimizar-y-apagar.md, y ejecuta solo lo que el dueño aprueba, verificando en vivo. Usar con "/optimizar", "qué apagamos", "qué escalamos".
---

# Optimizar

1. Leé `NEGOCIO.md`, `criterio/04-optimizar-y-apagar.md`, `criterio/06-trampas-de-la-api.md` y
   `bitacora.md` (qué se apagó y cuándo: el reloj de cada campaña sale de ahí y del log de la cuenta).
2. Traé por anuncio, de toda la cuenta, 4d y 7d: gasto, conversaciones, costo por conversación,
   frecuencia 7d, fecha de creación. Agrupá por post_id. Sumá clientes del registro si hay.
3. Aplicá la tabla del criterio. No toques lo lanzado hace menos de 2 días.
4. Presentá **una sola tabla** con decisión y porqué. Recordá que en CBO apagar no baja el gasto.
   Si querés bajar gasto, proponé bajar presupuesto con el monto exacto.
5. Esperá un "sí" explícito. Ejecutá solo lo aprobado, por `ad_id`.
6. Releé en vivo cada entidad tocada y reportá el estado real (no el de la respuesta de escritura).
7. Anotá en `bitacora.md`: fecha · ids · qué se hizo · por qué · cuándo volver a mirar.
