# 04 · Optimizar y apagar

## Ventanas

- **Últimos 4 días cerrados**: deciden.
- **Últimos 7 días**: dan contexto (¿viene mejorando o empeorando?).
- **Nunca el histórico de vida**: una campaña puede tener un promedio lindo y llevar 3 días sin
  traer un mensaje, o al revés.

## Cuándo se juzga

- Lo lanzado hace **menos de 2 días no se toca** (Meta está aprendiendo).
- Desde los **2-3 días** ya se puede decidir. Un ganador se nota en los primeros días.
- Después de apagar anuncios dentro de una campaña, se le dan **~4 días** antes de juzgar la
  campaña entera: el presupuesto pasa a otros anuncios que quizás nunca gastaron.

## Cuándo se apaga un anuncio (por `ad_id`)

Usando el costo máximo por conversación de `NEGOCIO.md` (lo llamamos "la vara"):

| Situación en 4 días | Decisión |
|---|---|
| Gastó ~2 varas y **0 conversaciones** | Apagar |
| Costo por conversación > 1,5 varas y el 7d no lo salva | Apagar |
| Trae conversaciones baratas pero el registro dice que **nunca cierran** | Apagar (o cambiar el texto) |
| Costo por conversación ≤ vara | Dejar |
| Costo ≤ 0,6 vara y cierra clientes | Ganador: candidato a escalar o a pasar a la campaña principal |
| Gastó muy poco (Meta no le da bola) | No se juzga: no tuvo oportunidad |

Con registro de clientes, la vara que manda es el **costo por cliente**; las conversaciones
pasan a ser diagnóstico.

## Antes de apagar una campaña entera

Se optimiza **adentro** primero. La propuesta tiene que mostrar:
1. cuándo se apagó el último anuncio,
2. cuántos siguen prendidos,
3. si se viene optimizando.

Si se apagó un anuncio en los últimos 4 días, la campaña no se apaga: se propone el próximo
anuncio. Excepción: una campaña que gastó mucho (≥ 5 varas en 4 días) sin traer nada.

Una campaña con frecuencia 7d baja (≈1,1) está llegando a gente nueva: más paciencia.

## Escalar

- Ganador claro 4d y 7d → subir presupuesto 20-30% o pasar el anuncio (mismo `post_id`) a la
  campaña principal.
- Después de subir, medir el escalón: si en 4 días el costo por conversación aguantó, se puede
  volver a subir.

## Cómo presenta Claude una propuesta

Tabla con: anuncio · `ad_id` · gasto 4d · conversaciones 4d · costo por conversación 4d · lo
mismo en 7d · frecuencia 7d · clientes registrados · decisión propuesta · por qué.
Nada se ejecuta sin un "sí" del dueño a esa tabla. Después de ejecutar, se relee en vivo.
