# 06 · Trampas del MCP de Meta (aprendidas a los golpes)

Para Claude. Cosas que pasan de verdad al escribir en Meta por el MCP.

1. **`success: true` no significa que se aplicó.** Siempre releer con `ads_get_ad_entities`.
2. **El borrador silencioso.** `ads_update_entity` puede dejar el cambio en borrador
   (`is_draft: true`) sin aplicarlo. Para que tome hay que publicarlo con `ads_activate_entity`
   pasando los ids:
   - pausar algo → `publish_as_active: false`
   - editar algo que estaba activo (ej. presupuesto) → `publish_as_active: true`, porque el
     cambio lo fuerza a pausa.
3. **`ads_activate_entity` puede devolver ACTIVE y la entidad quedar PAUSED.** Releer.
   `PUBLISHING` significa "entregado al publicador", no "publicado".
4. **`start_time` en el pasado se descarta en silencio.** El conjunto tiene su propio
   `start_time`: mover el de la campaña no lo arrastra.
5. **Anuncios con el mismo nombre.** Apagar por `ad_id`, nunca por nombre.
6. **El mismo posteo en varias campañas.** Para juzgar un anuncio, agrupar por
   `effective_object_story_id` (post_id) en toda la cuenta.
7. **Ubicación**: un targeting con solo país, sin `targeting_automation` explícito, puede salir
   distinto a lo esperado. Para negocio local, siempre radio o ciudades explícitas y releer el
   conjunto creado.
8. **Barridos de cuenta paginan.** Si la respuesta trae siguiente página, seguir hasta el final
   antes de sacar conclusiones.
9. **El video que devuelve el creativo** puede tener otro `video_id` que el subido: Meta publica
   su propia copia. No es error.
