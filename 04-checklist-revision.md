# Checklist · ¿Qué le falta a este prototipo para ser una app de verdad?

Para la práctica 3 (15 minutos, por parejas). Abrís desde el tablero el prototipo **de la pareja siguiente** (la 1 el de la 2, la 2 el de la 3… y la última el de la 1) y lo usáis como si fuerais el técnico de ITV. No hace falta saber programar: todo se comprueba haciendo clic.

---

## En clase: haz de técnico

Recorre su prototipo con clics, de principio a fin, y contesta estas tres preguntas:

1. **¿Sé qué me falta?** En 5 segundos, ¿veo qué campos tengo que revisar todavía?
2. **¿De dónde sale este dato?** ¿Puedo ver en qué parte del documento lo ha leído la IA, o tengo que fiarme?
3. **¿Puedo imprimir algo mal?** ¿Me deja imprimir con un aviso sin decidir o con datos viejos?

Después, en un **post-it del tablero**, junto a su prototipo, apuntad **3 cosas que le faltan para ser una app de verdad**. Mejor si al menos una no os la ha dicho la IA.

Ideas si os atascáis: qué pasa si algo falla (la impresora, el documento, la conexión), qué ve el técnico mientras la IA tarda, qué pasa con lo que pidió el cliente en la ronda 3, una tarjeta con 70 datos en vez de 16.

---

## Ayuda: las cinco preguntas antes de fiarte

Si queréis mirar más a fondo (en clase o en casa), estas son las cinco preguntas de la slide, con una forma rápida de comprobar cada una.

| Pregunta | Cómo lo compruebo |
|---|---|
| **Estructura** · ¿y si está vacío, cargando o da error? | Busca un campo vacío, una pantalla de espera y un mensaje de error. Si no hay, falta. Haz el recorrido también hacia atrás y apunta cada botón que no hace nada |
| **Accesibilidad** · ¿se lee bien? ¿avisa solo con colores? | Solo detectar (la veréis a fondo en su clase). Haz una captura en blanco y negro: ¿sigues sabiendo qué campo es dudoso? El contraste se mide con **WebAIM Contrast Checker** o el plugin **Stark**, nunca a ojo: mínimo 4,5:1 para texto y 3:1 para iconos y bordes |
| **Rendimiento** · ¿y si tarda un minuto? ¿y con 70 datos? | ¿Qué ve el técnico mientras espera: dice qué pasa o solo gira? Mete un valor larguísimo en un campo: ¿se corta, se desborda o rompe la fila? |
| **Mantenimiento** · ¿usa tus colores o se los inventa? | Pide a la IA la lista de colores que ha usado y compárala con el brief. Si mañana cambia el verde, ¿se toca en un sitio o en cuarenta? |
| **Fidelidad** · ¿se parece a lo que dibujaste? | Su frame del tablero al lado de su prototipo: el juego de las siete diferencias (letras, espacios, colores, estados, lo que añadió o quitó) |

Un dato para la de accesibilidad: los tres colores de confianza del brief (`#4AB586`, `#E89672`, `#FF6961`) dan entre 2,3 y 2,8:1 sobre blanco. No llegan ni al 3:1 de un icono.

---

**Regla final:** que se vea bien no significa que esté bien.
