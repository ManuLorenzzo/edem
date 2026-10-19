# Del diseño al prototipo navegable

**Tú diseñas y decides. Claude te asiste. Make lo hace funcionar.**

Make y los planes B y C funcionan con Figma gratis y Claude gratis. ⚠️ La ronda 1 (Claude crea en vuestro Figma) está probada con Claude de pago y Figma gratis, no con Claude gratis: si en vuestra pareja no funciona, usad la cuenta de una pareja con Claude de pago o pedid al profesor que lance vuestro prompt en pantalla. Si algo se atasca más de 5 minutos, pasad al plan B. Datos verificados el 19 oct 2026.

---

## El flujo: tres rondas y una entrega

Cada ronda dura unos 15 minutos: el profesor arranca en pantalla, vosotros trabajáis unos 10 y paramos 3 para ver resultados (`01-brief-mint-scan.md`, «Cómo va la práctica 2»). Solo se proyecta desde el portátil del profesor: en cada parada abre lo que hayáis pegado en **vuestro hueco del tablero de la clase** (enlace en la portada del kit).

| Ronda | Dónde | Qué hacéis | Ojo con |
|---|---|---|---|
| **1 · Rediséñalo con Claude** | Claude, con el conector de Figma | Pegáis el prompt de la ronda 1 con **vuestro dolor** (uno por pareja, `01-brief-mint-scan.md`); Claude crea el rediseño en vuestra copia con los componentes y variables que ya existen (`02-guia-figma-claude.md`, paso 4) y lo retocáis a mano. **Un frame, un dolor. No tiene que quedar perfecto.** Antes de la parada (17:32), pegáis en el tablero el enlace de vuestra copia del Figma, con permiso Ver (abajo) | Pedid "sin capturas de comprobación": escribir no gasta lecturas, leer sí. Permitir una vez en cada paso |
| **2 · Hazlo funcionar en Make** | Figma Make, en su propio chat | Copiáis **vuestro frame**, lo pegáis en el chat de Make con **un solo prompt** (el de la ronda 2, abajo) y, cuando acaba (unos 3 minutos), lo probáis con clics. **En cuanto funcione, lo publicáis** y pegáis el enlace del prototipo en el tablero (abajo) | Créditos (ver abajo). Modelo por defecto. Un frame por prompt. Mientras genera, apuntad qué vais a probar |
| **3 · El cliente cambia de idea** | **El mismo chat de Make** | Le pedís el cambio del cliente a Make, no a Claude: el prototipo vive en Make. Después, volvéis a publicar: el enlace es el mismo | Cambiad solo lo necesario. Después, repetid un clic de antes: ¿sigue funcionando? |
| **Entrega · 3 min** | Make y el tablero | Publicáis la versión final, y comprobáis que vuestro enlace abre en una ventana de incógnito | Con Figma gratis queda público en la Community: no pasa nada |

Claude, con el conector, **solo diseña en Figma**: lo que crea es diseño, no funciona. **Figma Make es otra herramienta**, con su propia IA, que convierte un frame en una app pequeña que funciona. Claude no maneja Make.

Después, en la práctica 3, revisáis el prototipo **de otra pareja** con Claude, en una conversación nueva, con cinco preguntas (`05-prompt-revision.md`). La IA tiende a dar por bueno lo que ve: pedidle "Demuéstralo". Y lo que se queda, se cambia o se pregunta al equipo técnico lo decidís vosotros: la IA no decide.

## Créditos de Figma Make: un prompt, bien hecho

Datos de la ayuda de Figma:

| | Cuánto |
|---|---|
| Hacer interactivo un diseño adjunto | **Unos 75 créditos o más** por prompt |
| Generar desde cero, sin diseño | **Unos 100 créditos o más** por prompt |
| Plan gratis (Starter) | **150 al día y 500 al mes**: unos **2 prompts al día por persona** |
| Education | 3.000 al mes |
| Modelo distinto del predeterminado | Gasta más. **Dejad el modelo por defecto** |

Estrategia de la pareja:

1. **Usad el prompt de la ronda 2 tal cual**, con vuestro dolor: en Make no se itera a base de probar.
2. **Una persona construye** en Make: un prompt en la ronda 2 y otro en la ronda 3, en el mismo chat.
3. **Los créditos de la otra persona son la reserva** por si se acaban. ⚠️ Compartidle el archivo de Make con permiso de edición y comprobad que puede escribir en él antes de necesitarlo.
4. ¿Cuánto me queda? Menú principal de Figma > **AI balance**.

Cómo darle vuestro diseño a Make:

- **Seleccionad vuestro frame en Figma, copiadlo y pegadlo en el chat de Make.** Un frame por prompt: el editor; la pantalla de éxito se describe en el texto del prompt.
- **Pegar la URL del archivo no sirve**: Make no lo lee así.
- Si al pegar el frame da error (fallo conocido), usad "Attach design" en el chat de Make.

**Motor ≠ herramienta**: Make deja elegir modelo de Anthropic, OpenAI o Google, pero la misma IA por debajo da resultados distintos según la herramienta que la envuelve. Aquí, modelo por defecto y a correr.

## Plan B · Fuera de Figma Make

| Vía | Qué es | Úsala si... | Ojo con |
|---|---|---|---|
| **Artifact de Claude** | Exportáis el frame como PNG y Claude lo convierte en una miniaplicación con enlace público | Os quedáis sin créditos de Make o Make falla | Claude ve una imagen, no las capas: colores y medidas aproximados |
| **Claude Design** | La herramienta de diseño de Claude, incluida en Claude gratis | Queréis explorar otra versión rápido | No exporta a Figma. Se aleja de vuestro sistema de diseño si no se lo dais |

## Plan C · Sin créditos ni IA: prototipo nativo de Figma

Conectad los frames con la pestaña **Prototipo** de Figma (de un botón del editor a la pantalla de éxito) y pulsad Presentar. No gasta créditos ni mensajes. No es código, pero es navegable y sirve para la puesta en común y para revisar con la checklist. Es el plan de la ronda 2 si Make falla.

## Cómo publicar y compartir

Todo va a **vuestro hueco del tablero de la clase**, que el profesor proyecta desde su portátil (`01-brief-mint-scan.md`, «Qué entregáis y dónde»):

| Cuándo | Qué pegáis |
|---|---|
| Ronda 1, antes de la parada de las 17:32 | El enlace de vuestra copia del Figma |
| Ronda 2, en cuanto el prototipo funcione | El enlace del prototipo de Make (`.figma.site`) |
| Ronda 3 | Nada nuevo: volvéis a publicar y el enlace es el mismo |
| Entrega (3 min) | Versión final publicada y enlace comprobado en incógnito |

### Ronda 1 · El enlace de vuestra copia del Figma

1. En vuestra copia, pulsad **Compartir** (*Share*), arriba a la derecha.
2. En el acceso por enlace, elegid **«Cualquiera con el enlace»** con permiso **Ver**. Con Figma gratis se puede.
3. **Copiar enlace** y pegadlo en vuestro hueco del tablero.

### Rondas 2 y 3 · Figma Make, paso a paso

⚠️ Los nombres de los botones se comprueban en el ensayo: pueden cambiar o salir en inglés.

1. En vuestro archivo de Make, pulsad **Publicar** (*Publish*), arriba a la derecha. ⚠️
2. **Con Figma gratis (Starter)**, Make os pide publicarlo también en la **Community de Figma**: aceptad. Queda **público**, y no pasa nada: los datos son inventados. ⚠️ Si es la primera vez, puede pediros crear un perfil de Community (un minuto).
3. Al terminar os da una dirección que acaba en **`.figma.site`**. Copiadla con el botón de copiar enlace. ⚠️
4. Abridla en una ventana de incógnito o en el móvil: si se ve sin iniciar sesión, está bien.
5. Pegadla en vuestro hueco del tablero.

En la ronda 3, tras el cambio, **volved a publicar** desde el mismo botón ⚠️: la dirección no cambia, así que no hace falta pegarla otra vez.

Con **Education** se puede publicar 1 archivo sin pasar por la Community.

Si no hay manera de publicar: avisad al profesor; la pareja que os revise lo probará en vuestro portátil.

### Las otras vías

- **Artifact de Claude**: botón **Publish** en el artifact; genera un **enlace público** que se abre sin cuenta.
- **Claude Design**: compartir desde Claude Design o capturas de cada pantalla. No exporta a Figma.
- **Prototipo de Figma**: **Compartir prototipo** con «cualquiera con el enlace puede ver» ⚠️ y copiar el enlace; si no, capturas.

Sea cual sea la vía, al tablero va **un enlace**: es lo que usará la pareja que os revise en la práctica 3.

---

## Las 5 C's en un prompt

| C | Qué significa |
|---|---|
| **Cabeza** | Quién eres y qué buscas |
| **Contexto** | El brief, el usuario, tu sistema de diseño |
| **Consultar** | "Antes de empezar, hazme las preguntas que necesites" |
| **Comprobar** | Cómo sabrás que está bien: criterios y qué no debe hacer |
| **Cortar** | Una pantalla cada vez |

---

## Prompt · Ronda 1 (Claude lo crea en vuestro Figma)

En Claude, con el conector de Figma activo y el enlace a vuestra copia del Figma de partida:

```
[pega aquí el enlace a vuestra copia del Figma de partida]

CABEZA: Soy diseñador de producto. Quiero que rediseñes en este archivo de Figma el editor de revisión de la Tarjeta ITV. Después lo retocaré yo a mano.

CONTEXTO: Un técnico de ITV experto revisa de 40 a 70 campos que propone una IA, con el documento original al lado, en Windows a 1280 px o más, con atajos de teclado. Nos toca resolver este dolor: [pega vuestra fila de la tabla del brief: «Le duele…»]. No se toca el sistema de diseño de Mint.

CONSULTAR: Solo si te falta algo imprescindible, hazme una pregunta antes de crear. Si no, empieza: tenemos 10 minutos.

COMPROBAR: El rediseño tiene que cumplir esto: [pega vuestra columna «Sabremos que está resuelto si…»]. Usa solo los componentes y variables que ya existen (Fila de campo, Insignia de confianza, Alerta, Botón, Chip de aviso); no inventes colores ni componentes. Sin capturas de comprobación. Al terminar, dime qué has creado y qué no has podido resolver con el sistema.

CORTAR: Crea un solo frame nuevo "Editor · rediseño" al lado del Editor, sin tocar el original. Solo el editor.
```

Abrid Figma y **retocadlo a mano**: lo que decidís vosotros, no Claude. Si queréis otro cambio, una petición concreta cada vez: *"En el frame Editor · rediseño, cambia solo [esto]. Sin capturas de comprobación."* No tiene que quedar perfecto: a los 10 minutos paramos.

## Prompt · Ronda 2 (Figma Make)

Copiad el frame "Editor · rediseño" en Figma, pegadlo en el chat de Make, dejad el modelo por defecto y pegad este prompt con vuestro dolor:

```
CABEZA: Convierte el frame pegado en un prototipo navegable de 2 pantallas para un técnico de ITV.

CONTEXTO: (1) El editor del frame: el técnico revisa de 40 a 70 campos que propone una IA, cada uno con confianza (alta, media, baja), documento de origen y, a veces, una alerta. Se puede marcar un campo como revisado y aceptar o corregir una alerta. Un contador dice cuántos campos faltan. Este diseño resuelve este dolor y tiene que poder probarse con clics: [vuestro dolor]. El botón Imprimir lleva a (2) una pantalla de éxito con la vista previa de la tarjeta y la confirmación. Escritorio, 1280 px o más. Usa los datos del frame.

COMPROBAR: Respeta el frame: tipografía, espaciados, colores (verde #4AB586, confianza alta #4AB586, media #E89672, baja #FF6961, Inter, JetBrains Mono) y estados. No inventes campos, colores ni componentes. No dejes imprimir con alertas sin decidir. Al terminar, dime qué no has podido respetar y qué datos te has inventado.

CORTAR: Solo estas 2 pantallas.
```

Sin "Consultar" en Make: cada respuesta gasta créditos. Mientras genera (unos 3 minutos), apuntad qué clics vais a hacer para probar vuestro dolor.

## Prompt · Ronda 3 (el cambio, en el mismo chat de Make)

El cambio lo cuenta el profesor en pantalla. Escribidlo en el **mismo chat de Make**, no en uno nuevo ni en Claude:

```
El cliente pide este cambio: [lo que pide el cliente, de la slide].

Aplícalo a nuestro dolor: [vuestro dolor]. Cambia solo lo necesario y no rompas lo que ya funcionaba: marcar campos como revisados, el contador, las alertas y el paso a la pantalla de éxito. Al terminar, dime qué has cambiado y qué no has podido resolver.
```

Después, repetid un clic de los de antes: ¿sigue funcionando?

## Prompt · Práctica 3 (Claude revisa)

Está en `05-prompt-revision.md`.

## Prompt · Plan B (artifact de Claude)

Exportad el frame como PNG a 2x, arrastradlo al chat de Claude y pegad:

```
CABEZA: Soy diseñador de producto. Convierte esta imagen en un prototipo navegable como artifact.

CONTEXTO: Es el editor donde un técnico de ITV revisa los campos que propone una IA. Que se pueda hacer clic: marcar campos como revisados, aceptar o corregir alertas e ir a una pantalla de éxito tras imprimir. Datos ficticios: [pega la tabla del brief]. Copia el estilo de la imagen: verde #4AB586, confianza alta #4AB586, media #E89672, baja #FF6961, Inter.

CONSULTAR: Antes de construirlo, hazme las preguntas que necesites. Máximo 3.

COMPROBAR: No inventes campos ni colores. Al terminar, lista lo que has tenido que suponer porque no se veía en la imagen.

CORTAR: Primero solo el editor, funcionando. Luego la pantalla de éxito.
```

Para **Claude Design**, el mismo prompt cambiando la primera línea por: *"CABEZA: Soy diseñador de producto y necesito 2 variantes del editor de revisión de una Tarjeta ITV para un prototipo navegable."*

---

**Después de clase:** si vais a usar Make con vuestros propios diseños, preparad antes el prompt con Claude, que no gasta créditos de Make: *"Necesito escribir un único prompt para Figma Make. Te paso mi diseño y lo que quiero que haga. Antes de escribirlo, hazme hasta 3 preguntas. Devuélveme solo el prompt, en menos de 200 palabras."*

**Truco:** si no sabes cómo pedir algo, pídeselo a ella: *"Quiero conseguir X con este diseño. Escríbeme el mejor prompt para pedírtelo."* El mejor prompt te lo escribe ella.
