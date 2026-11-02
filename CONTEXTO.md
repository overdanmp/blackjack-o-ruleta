# Contexto: Blackjack y apuestas deportivas

Resumen para continuar la conversación en otro chat. Última actualización: 2 de noviembre de 2026.

---

## 1. Quién es el usuario y cómo quiere que le respondan

- **Idioma:** español. Está en **Colombia** (hora UTC-5) y juega en **pesos colombianos (COP)**.
- **Casa de apuestas:** BetPlay (casino en vivo y deportes).
- **Estilo de respuesta:**
  - Respuestas cortas y concisas, sin párrafos largos.
  - Un paso a la vez: una idea, una pregunta y esperar respuesta.
  - Lenguaje simple, sin términos enredados.
  - Terminar casi siempre con **una sola pregunta concreta**.
  - Si pide un archivo, dárselo primero.
  - Cuando corrige, aceptar. Si hay un argumento real en contra, decírselo con respeto, sin ceder por complacencia.
- **Cómo pide ayuda:** manda capturas de pantalla de cada mano o de su cupón de apuestas, y espera la jugada exacta o una opinión directa.
- **Su forma de jugar:**
  - Le gusta ponerse metas ("hacer 20k", "hacer 30k").
  - A veces sube la apuesta después de perder.
  - Suele armar combinadas de muchos partidos.
  - Acepta bien los consejos de retirarse cuando va ganando.

---

## 2. La verdad matemática que se le ha explicado

- **Ruleta:** no se le puede ganar a largo plazo. Ningún sistema (Martingala, etc.) cambia la ventaja de la casa.
- **Blackjack en línea (RNG / First Person):** baraja cada mano, así que **contar cartas no sirve**. Con estrategia básica perfecta, la casa tiene ~0.5% a favor: es casi una moneda al aire.
- **Apuestas deportivas:**
  - Cada cuota trae el margen de la casa (~5%).
  - En una combinada, ese margen se multiplica y la chance real cae rápido.
  - Lo que mejor le ha funcionado son las apuestas de **1 o 2 partidos**.
- **Retirarse siempre es la jugada correcta en números**, porque cada mano o apuesta extra tiene expectativa negativa.

La guía completa de estrategias está en `GUIA.md` (mismo repositorio).

---

## 3. Reglas que usamos al jugar blackjack

1. **Antes de empezar:** fijar una **meta** de ganancia y un **límite de pérdida**.
2. Usar una **apuesta fija** por mano (5.000 o 10.000). **No subirla para recuperar.**
3. **Nunca:** tomar seguro, hacer apuestas laterales (Poker, Pairs, 21+3) ni jugar mesas que paguen 6:5.
4. **Botón "Cobrar" (Evolution):** comparar su valor con el valor esperado de jugar la mano. Casi siempre conviene jugar.
5. Al llegar a la meta o al límite, **se retira**.

**Chances de llegar a la meta antes del límite (aprox.):**

| Meta | Límite | Chance |
|---|---|---|
| +20.000 | −20.000 | ~50% |
| +20.000 | −40.000 | ~66% |
| +30.000 | −40.000 | ~56% |
| +30.000 | −60.000 | ~65% |

**Estrategia básica resumida:**
- 17 o más: plantarse.
- 13–16: plantarse contra 2–6; pedir contra 7–As.
- 12: plantarse contra 4–6; si no, pedir.
- 11: doblar (salvo contra As).
- 10: doblar contra 2–9.
- 9: doblar contra 3–6.
- Dividir siempre As-As y 8-8. Nunca 5-5 ni 10-10.
- Blandas: A+7 se planta contra 2–8. A+8 y A+9 se plantan.

**Herramienta:** el script `ev.py` (en el scratchpad de la sesión) calcula el valor esperado de pedir o plantarse con mazo infinito, y el crupier se planta en 17 suave. Se usó para comparar contra "Cobrar".

### Mesas que ha usado

| Mesa | Proveedor | Mínimo | Detalles |
|---|---|---|---|
| First Person Blackjack | Evolution | 2.500 | Paga 3:2, crupier se planta en 17, tiene "Cobrar" |
| Classic Blackjack | Espresso | 500 | Mesa azul de BetPlay |
| Blackjack Poker and Pairs | — | 500 | Tiene apuestas laterales, no usarlas |

---

## 4. Historial de saldo y resultados

| Fecha | Qué pasó | Resultado |
|---|---|---|
| 15 oct | Blackjack de 20.426 a 40.426, con apuestas de 5.000 | +20.000 |
| 17 oct | Blackjack de 40.426 a 60.426, con apuestas de 10.000. Se retiró antes de su meta de 70.000 | +20.000 |
| 17 oct | Apuestas de fútbol. Rechazó apostar 60.000 a una combinada de 7 partidos. Mostró una de 6 partidos (cuota 14.68) por 15.000 | Resultado no reportado |
| 20 oct | Champions: 5 apuestas. Ganó una doble de goles (70.000 → 134.400) y una sencilla a PSG con apuesta gratis. Perdió 3 combinadas, casi todas por Porto | **+28.800** (saldo ~141.800) |
| 21 oct | Blackjack de ~142.400 a 152.400. Paró | +10.000 |
| 21 oct | Se le recomendaron apuestas de Champions (Inter, combinadas con córners y goles) | Resultado no reportado |
| 21 oct | Blackjack (Poker & Pairs y Evolution): de 126.438 bajó a 111.438 y se recuperó a 127.688 | +1.250 |
| 21 oct | **Retiró 100.000 al banco** | — |
| 21 oct | Jugó con ~27.700 y llegó a 32.688 (ganó 4 manos a la vez) | +5.000 |
| 31 oct | Blackjack de 38.638 a 53.638, apuesta de 5.000. Paró antes de su meta de +20.000 | +15.000 |
| 31 oct | Combinada de 4 partidos, 9.000 a cuota 11.69: Roma, Inter, Chelsea y Man City ganan. Pago potencial 105.191 | **Pendiente / no reportado** |

**Último saldo conocido:** ~53.638 en BetPlay antes de la combinada de 9.000 (quedarían ~44.638). Más los **100.000 retirados al banco**.

---

## 5. Lecciones que han funcionado

- **Retirarse a tiempo:** sus mejores días fueron cuando paró al llegar a la meta o un poco antes.
- **Retirar ganancias al banco:** lo hizo con 100.000 y quedaron a salvo.
- **Apuestas cortas (1 o 2 partidos):** ganó todas las de 1 o 2 patas el 20 de octubre y perdió todas las de 3 o más.
- **No perseguir pérdidas:** cuando subió la apuesta después de perder, terminó más abajo.
- **Jugar varias manos a la vez** no mejora la chance, solo acelera las subidas y bajadas.

---

## 6. Cómo ayudarle en el próximo chat

1. Preguntar primero **saldo actual** y **resultado de la combinada de 9.000** (31 oct).
2. **Si quiere jugar blackjack:**
   - Fijar meta y límite antes de empezar.
   - Indicarle la jugada en cada captura.
   - Llevar la cuenta del saldo.
   - Recordarle retirarse al llegar a la meta o al límite.
3. **Si quiere apostar en deportes:**
   - Buscar partidos y cuotas del día; las horas, en hora Colombia.
   - Ordenar las apuestas de más probable a menos.
   - Dar la chance real aproximada de cada combinada.
   - Recomendar apuestas de pocos partidos y no meter todo el saldo.
   - Citar las fuentes.
4. Ser honesto: ninguna apuesta es segura. Respetar su decisión, pero mostrarle siempre los números.
