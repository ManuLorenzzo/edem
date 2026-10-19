# 4 · ¿Qué le falta?

Práctica 3, por parejas. No hace falta saber programar: todo se comprueba con clics.

## 1 · Abre el prototipo de la pareja siguiente

Desde el tablero. La 1 revisa el de la 2, la 2 el de la 3… y la última, el de la 1.

## 2 · Haz de técnico

Recórrelo de principio a fin y contesta:

1. **¿Sé qué me falta?** En 5 segundos, ¿veo qué campos me quedan por revisar?
2. **¿De dónde sale este dato?** ¿Veo en qué parte del documento lo leyó la IA, o tengo que fiarme?
3. **¿Puedo imprimir algo mal?** ¿Me deja imprimir con un aviso sin decidir o con datos viejos?

## 3 · Apunta 3 cosas

En las **casillas rosas de su columna del tablero** (la de la pareja que revisas): **3 cosas que le faltan para ser una app de verdad.** Mejor si al menos una no te la ha dicho la IA.

¿Atascado? Piensa en qué pasa si falla la impresora, qué ve el técnico mientras la IA tarda, una tarjeta con 70 datos en vez de 16, o el cambio del cliente de la ronda 3.

## Ayuda: cinco preguntas antes de fiarte

| Pregunta | Cómo lo compruebas |
|---|---|
| **Estructura** · ¿y si está vacío o da error? | Busca un campo vacío, una espera y un error. Apunta cada botón que no hace nada |
| **Accesibilidad** · ¿se lee bien? ¿avisa solo con colores? | Solo detectar. Míralo en blanco y negro: ¿sigues viendo qué dato es dudoso? El contraste se mide con WebAIM Contrast Checker, nunca a ojo (los tres colores de confianza dan entre 2,3 y 2,8:1 sobre blanco; el mínimo de un icono es 3:1) |
| **Rendimiento** · ¿y si tarda un minuto? ¿y con 70 datos? | ¿Qué ve el técnico mientras espera? Mete un valor larguísimo: ¿rompe la fila? |
| **Mantenimiento** · ¿usa tus colores o se los inventa? | Compara sus colores con los del Figma. Si mañana cambia el verde, ¿se toca en un sitio o en cuarenta? |
| **Fidelidad** · ¿se parece a lo que dibujaron? | Su Figma (enlace en el tablero) al lado del prototipo: el juego de las siete diferencias |

## Opcional: que Claude te dé ideas

En una **conversación nueva** (la IA que lo hizo tiende a defenderlo), con capturas o con su enlace. El prompt lo escribes tú: dile qué es y cuál era su dolor, **pídele que lo revise con las cinco preguntas** de arriba y que te dé las 3 cosas que más le faltan.

Con lo que te parezca raro, **pídele que te demuestre cada fallo**: en qué pantalla, en qué elemento y con cuánta seguridad.

Lo que diga Claude se comprueba con clics, no se copia. Lo que no sepa demostrar, fuera.

**Que se vea bien no significa que esté bien.**
