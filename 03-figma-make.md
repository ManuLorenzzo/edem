# 3 · Figma Make, ronda a ronda

Claude, con el conector, **solo diseña en Figma**. **Figma Make** es otra herramienta, con su propio chat, que convierte tu frame en una app pequeña que funciona. Desde la ronda 2, todo se pide en Make.

## Ronda 2 · Hazlo funcionar

1. En Figma, **selecciona tu frame «Editor · rediseño» y cópialo**. Pegar el enlace del archivo **no sirve**: Make no lo lee.
2. Abre Figma Make y **pega el frame en su chat**. Si da error al pegar (fallo conocido), usa «Attach design».
3. Deja el **modelo por defecto** (los otros gastan más créditos).
4. Pega este prompt con tu dolor y envíalo:

```
CABEZA: Convierte el frame pegado en un prototipo navegable de 2 pantallas para un técnico de ITV.

CONTEXTO: (1) El editor del frame: el técnico revisa de 40 a 70 campos que propone una IA, cada uno con confianza (alta, media, baja), documento de origen y, a veces, una alerta. Se puede marcar un campo como revisado y aceptar o corregir una alerta. Un contador dice cuántos campos faltan. Este diseño resuelve este dolor y tiene que poder probarse con clics: [tu dolor]. El botón Imprimir lleva a (2) una pantalla de éxito con la vista previa de la tarjeta y la confirmación. Escritorio, 1280 px o más. Usa los datos del frame.

COMPROBAR: Respeta el frame: tipografía, espaciados, colores (verde #4AB586, confianza alta #4AB586, media #E89672, baja #FF6961, Inter, JetBrains Mono) y estados. No inventes campos, colores ni componentes. No dejes imprimir con alertas sin decidir. Al terminar, dime qué no has podido respetar y qué datos te has inventado.

CORTAR: Solo estas 2 pantallas.
```

5. Tarda unos 3 minutos. Mientras, apunta qué clics vas a hacer para probar tu dolor. Luego, pruébalo.

## Publica y copia el enlace

⚠️ Los nombres de los botones pueden cambiar o salir en inglés.

1. Pulsa **Publicar** (*Publish*), arriba a la derecha. ⚠️
2. Con Figma gratis te pide publicarlo también en la **Community de Figma**: acepta. Queda público y no pasa nada, los datos son inventados. ⚠️ La primera vez puede pedirte crear un perfil (un minuto).
3. Copia la dirección que acaba en **`.figma.site`** con el botón de copiar enlace. ⚠️
4. Ábrela en una ventana de incógnito: si se ve sin iniciar sesión, está bien.
5. Pégala en tu hueco del tablero. **Solo el enlace, sin capturas.**

## Créditos: un prompt, bien hecho

Con Figma gratis te llegan para **unos 2 prompts al día**. Así que:

- **Una persona de la pareja construye**: un prompt en la ronda 2 y otro en la ronda 3, en el mismo chat.
- **Los créditos de tu compañero son la reserva.** ⚠️ Compártele el archivo de Make con permiso de edición y comprueba que puede escribir antes de necesitarlo.

## Ronda 3 · El cliente cambia de idea

El cambio te lo cuento en pantalla. Pídeselo a Make **en el mismo chat**, no en uno nuevo ni en Claude:

```
El cliente pide este cambio: [lo que pide el cliente, de la slide].

Aplícalo a nuestro dolor: [tu dolor]. Cambia solo lo necesario y no rompas lo que ya funcionaba: marcar campos como revisados, el contador, las alertas y el paso a la pantalla de éxito. Al terminar, dime qué has cambiado y qué no has podido resolver.
```

Repite un clic de los de antes: ¿sigue funcionando? Luego **vuelve a publicar** con el mismo botón. El enlace no cambia: no hace falta pegarlo otra vez.

## Plan B: si Make falla o te quedas sin créditos

No pierdas más de 5 minutos. Usa el **prototipo de Figma de siempre**: en la pestaña **Prototipo**, conecta el botón Imprimir del editor con una pantalla de éxito y pulsa Presentar. No gasta créditos.

Para el tablero: **Compartir prototipo**, «Cualquiera con el enlace puede ver» ⚠️, y pega el enlace.
