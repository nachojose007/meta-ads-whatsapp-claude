# 05 · WhatsApp: la mitad del resultado

El anuncio consigue que alguien escriba. **Que se anote depende de lo que pasa en el chat.**

## Configuración (una vez)

1. **WhatsApp Business** (la app gratis) con el número del estudio.
2. Conectar el número a la **página de Facebook**: Página → Configuración → Cuentas vinculadas
   → WhatsApp. Sin esto no se pueden crear anuncios a WhatsApp.
3. En WhatsApp Business → Herramientas para la empresa:
   - **Perfil**: dirección, horario, Instagram, descripción corta.
   - **Mensaje de bienvenida**: corto, humano, con una pregunta. Ej: "¡Hola! Soy Mati de
     [estudio] 🙌 ¿Ya hiciste yoga alguna vez o sería tu primera clase?"
   - **Mensaje de ausencia** fuera de horario, diciendo cuándo vas a contestar.
   - **Respuestas rápidas**: horarios (/horarios), precios (/precios), cómo llegar (/llegar),
     qué traer (/traer).
   - **Etiquetas**: `Anuncio`, `Agendó prueba`, `Vino`, `Se anotó`, `No respondió`.
4. En el anuncio: **mensaje precargado** ("¡Hola! Quiero reservar mi clase de prueba") para
   reconocer que viene de publicidad.

## La regla de los 5 minutos

La probabilidad de cerrar cae muy rápido con el tiempo de respuesta. Alguien que escribió desde
un anuncio está mirando el teléfono **ahora**. Si contestás 3 horas después, ya está en otra.
- Prender los anuncios **solo en el horario en que alguien puede contestar** (programación de
  anuncios por horario, o apagar de noche) si no hay quien responda.
- Medir: de cada 10 conversaciones, ¿cuántas se contestaron en menos de 5 minutos?

## El guion del primer chat

1. Saludo + pregunta (¿primera vez? ¿qué te trae?).
2. Escuchar el motivo (espalda, estrés, moverse) y responder a eso, no tirar la lista de precios.
3. Ofrecer **una acción concreta**: "¿Te reservo la clase de prueba del jueves 19 h?"
4. Confirmar con día, hora, dirección y qué traer.
5. Recordatorio el día anterior.
6. Después de la clase: "¿Cómo te sentiste?" + propuesta de abono.

Precio: se da cuando lo piden, siempre junto con la clase de prueba como siguiente paso.

## Registrar para cerrar el círculo

Cada conversación de anuncio va a `registro/conversaciones.csv` (o se le cuenta a Claude con
`/registrar`): fecha, de qué anuncio vino (si se sabe), si respondió, si agendó, si vino, si se
anotó. Con eso Claude calcula el costo por cliente real de cada anuncio.

## Nivel 2 (opcional): leer el WhatsApp desde Claude Code

Existe un conector no oficial (`whatsapp-mcp`, de código abierto) que vincula WhatsApp como
"dispositivo" igual que WhatsApp Web, y le permite a Claude leer chats para armar el registro
solo, medir tiempos de respuesta y redactar respuestas. Cuidados:
- No es de Meta: usalo sabiendo que es un dispositivo vinculado más.
- Empezá **solo leyendo**. Que Claude redacte y vos mandes.
- Nunca mensajes masivos ni a gente que no te escribió: es la forma más rápida de que bloqueen
  el número.
