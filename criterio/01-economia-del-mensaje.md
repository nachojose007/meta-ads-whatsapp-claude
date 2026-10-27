# 01 · La economía del mensaje

En una tienda online, Meta ve la venta y se puede medir el ROAS. En un negocio que vende por
WhatsApp, **Meta solo ve que alguien empezó una conversación**. Lo que pasa después (si
contestó, si vino a la clase de prueba, si se anotó) pasa en tu teléfono, no en Meta.

Por eso el criterio se arma con tres números y un registro.

## Los tres números

| Número | De dónde sale | Ejemplo yoga |
|---|---|---|
| Valor de un cliente nuevo | abono × meses promedio (tope 3) | $40.000 × 3 = $120.000 |
| % de conversaciones que cierran | registro de conversaciones | 15% |
| % del valor que pagás en publicidad | decisión del dueño | 30% |

```
Costo máximo por cliente      = 120.000 × 30%  = $36.000
Costo máximo por conversación = 36.000 × 15%   = $5.400
```

**Son el mismo dato escrito de dos formas.** Si el % de cierre cambia, cambia la vara por
conversación. Por eso un semáforo fijo de "costo por mensaje" no sirve: el mismo costo por
mensaje es excelente si cierran 3 de cada 10 y malo si cierra 1 de cada 20.

## La escalera de métricas (de arriba para abajo)

1. **Costo por cliente** (gasto ÷ clientes nuevos registrados) — el que manda.
2. **% de cierre** (clientes ÷ conversaciones) — dice si el problema es el anuncio o WhatsApp.
3. **Costo por conversación iniciada** (en Meta: *Conversaciones con mensajes iniciadas*) — el
   que Meta optimiza y el que se lee todos los días.
4. **Señales tempranas**: CTR saliente, costo por clic al botón de WhatsApp, % de video visto.
   Sirven para diagnosticar, **nunca para decidir solas**.

## Cuándo el problema NO es el anuncio

- Muchas conversaciones y pocos clientes → mirar primero cuánto tardan en contestar y qué se
  ofrece en el primer mensaje (ver `05-whatsapp.md`).
- Conversaciones de gente fuera de la zona → revisar la ubicación del conjunto (radio y
  "personas que viven en").
- Conversaciones que preguntan precio y desaparecen → el anuncio promete algo que el precio no
  sostiene, o el primer mensaje tira el precio sin ofrecer la clase de prueba.

## Cerrar el círculo

Cada conversación que llega por anuncio se anota en `registro/conversaciones.csv` (o se le
dice a Claude con `/registrar`). Con 2-3 semanas de registro se sabe qué anuncio trae
**clientes**, no solo mensajes. Sin registro, se optimiza a ciegas hacia el mensaje más barato,
que casi nunca es el mejor.
