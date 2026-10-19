# 2 · Claude y Figma

Objetivo: **escribes en Claude y aparece en tu Figma**, con tus componentes y tus variables. Basta una cuenta por pareja.

## Conectar (5 minutos)

1. **Lo más fácil: pídeselo a tu IA.** Escríbele «Conéctate al MCP de Figma y guíame» y te lleva paso a paso.
2. En **[claude.ai](https://claude.ai)** (cuenta gratis con tu email o con Google; ⚠️ puede pedir un móvil, si no quieres darlo usa la de tu pareja): **Ajustes > Conectores > Descubrir**, busca **Figma** y pulsa **Conectar**.
3. Se abre Figma: inicia sesión y pulsa **Aceptar y permitir el acceso**.
4. **Duplica el Figma de Mint Scan** (botón 3 de la página de la clase) **con la misma cuenta de Figma que has conectado**: menú del nombre del archivo > **Duplicar** ⚠️ (el texto del menú puede variar un poco). Si lo duplicas con otra cuenta, Claude no podrá crear nada.
5. En tu copia, **Compartir > Copiar enlace** y pega ese enlace en Claude al principio de cada petición.

Claude te pedirá permiso en cada paso: pulsa **Permitir una vez** y mira qué va a tocar.

Un MCP es un enchufe para que la IA use otra herramienta. Como un USB-C: el mismo conector para muchos aparatos.

⚠️ Probado con Claude de pago y Figma gratis. **Con Claude gratis, sin probar.** Si no crea nada: comprueba que has pegado el enlace de **tu copia** y que la cuenta conectada es la dueña. Si sigue sin ir en 5 minutos, únete a una pareja con Claude de pago o pídeme que lance tu prompt en pantalla.

⚠️ Claude gratis tiene pocos mensajes (Anthropic no da cifra; terceros estiman de 15 a 40 cada 5 horas). Prompts concretos y pocos; si se acaban, sigue con la cuenta de tu pareja.

## Cómo pedirlo: las 5 C

- **Cabeza:** quién eres y qué quieres.
- **Contexto:** el usuario, el objetivo y tu sistema de diseño.
- **Consultar:** «Antes de empezar, pregúntame lo que necesites».
- **Comprobar:** qué tiene que cumplir. Lo miras tú en Figma, no le pidas capturas: con Figma gratis tienes unas 20 lecturas al mes (crear no las gasta). Por eso los prompts acaban en «Sin capturas de comprobación».
- **Cortar:** una cosa cada vez. Nada de «rediséñalo todo».

## Práctica 1: elige un prompt (20 minutos)

Pega antes el enlace de tu copia. El archivo trae estos componentes: **Fila de campo**, **Insignia de confianza**, **Alerta**, **Botón** y **Chip de aviso**.

**Una variante**
```
Crea en este archivo una variante nueva de la Fila de campo, "Con alerta pendiente": borde ámbar y un aviso corto debajo del valor, usando los componentes y variables que ya existen. Sin capturas de comprobación.
```

**Una pantalla nueva**
```
Crea en la página Editor un frame nuevo de 1440x900 llamado "Editor · todo revisado". Usa instancias de la Fila de campo en variante Revisada y un Botón primario "Imprimir". Solo componentes y variables que ya existen. Sin capturas de comprobación.
```

**Un estado vacío**
```
Crea un frame "Editor · sin campos" para cuando la IA no ha podido leer ningún campo del documento: un mensaje, una línea que explique qué hacer y un Botón primario "Volver a escanear". Usa los componentes y variables que ya existen. Sin capturas de comprobación.
```

**Un aviso nuevo**
```
Añade al componente Alerta una variante nueva para "Sin conexión con la impresora", con las variables de aviso y la misma estructura que las otras variantes. Sin capturas de comprobación.
```

Abre Figma y míralo. ¿Ha usado tus componentes o se ha inventado otros?

## Ronda 1: rediseña tu dolor

Rellena los dos huecos con tu fila del encargo (documento 1):

```
[pega aquí el enlace a tu copia del Figma]

CABEZA: Soy diseñador de producto. Quiero que rediseñes en este archivo de Figma el editor de revisión de la Tarjeta ITV. Después lo retocaré yo a mano.

CONTEXTO: Un técnico de ITV experto revisa de 40 a 70 campos que propone una IA, con el documento original al lado, en Windows a 1280 px o más, con atajos de teclado. Nos toca resolver este dolor: [tu «Le duele…»]. No se toca el sistema de diseño de Mint.

CONSULTAR: Solo si te falta algo imprescindible, hazme una pregunta antes de crear. Si no, empieza: tenemos 10 minutos.

COMPROBAR: El rediseño tiene que cumplir esto: [tu «Sabremos que está resuelto si…»]. Usa solo los componentes y variables que ya existen (Fila de campo, Insignia de confianza, Alerta, Botón, Chip de aviso); no inventes colores ni componentes. Sin capturas de comprobación. Al terminar, dime qué has creado y qué no has podido resolver con el sistema.

CORTAR: Crea un solo frame nuevo "Editor · rediseño" al lado del Editor, sin tocar el original. Solo el editor.
```

Luego **retócalo a mano**: decides tú, no Claude. ¿Otro cambio? Uno cada vez: *«En el frame Editor · rediseño, cambia solo [esto]. Sin capturas de comprobación.»*

## Tus datos

Claude: puedes impedir que entrene con tus chats en **Ajustes > Privacidad**.
Figma **entrena con tus archivos por defecto** en el plan gratis y en Professional (en Education, no). Por eso hoy solo usamos datos inventados.

## Si usas Claude Code

```
claude mcp add --transport http figma https://mcp.figma.com/mcp
```

Añade `--scope user` para tenerlo en todos tus proyectos y escribe `/mcp` para iniciar sesión en Figma.
