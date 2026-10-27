---
name: registrar
description: Carga en registro/conversaciones.csv las conversaciones de WhatsApp que llegaron por anuncios y en qué terminaron (respondió, agendó, vino, se anotó), para calcular el costo por cliente real. Usar con "/registrar", "hoy escribieron 5 y se anotaron 2", o cuando el dueño cuenta cómo le fue con los chats.
---

# Registrar conversaciones

1. Pedile al dueño (o aceptá en texto libre) las conversaciones del día: cuántas llegaron por
   anuncio, de qué anuncio si se sabe (el mensaje precargado o la vista del anuncio en el chat
   ayudan), y en qué quedó cada una.
2. Agregá una fila por conversación a `registro/conversaciones.csv`. Nunca guardes nombres
   completos ni teléfonos: usá un alias corto (ej. "Laura P.").
3. Mostrá cómo quedó la semana: conversaciones, % que respondió, % que agendó, % que se anotó,
   y costo por cliente (gasto de Meta de esos días ÷ clientes).
4. Si el % de cierre de 2+ semanas difiere del de `NEGOCIO.md`, proponé actualizarlo (cambia la vara).
