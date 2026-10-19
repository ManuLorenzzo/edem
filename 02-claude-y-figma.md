# 2 · Claude y Figma

Objetivo: **escribes en Claude y aparece en tu Figma**, con tus componentes y tus variables. Basta una cuenta por pareja.

## Conectar

1. **Lo más fácil: pídeselo a tu IA.** Escríbele «Conéctate al MCP de Figma y guíame» y te lleva paso a paso.
2. En **[claude.ai](https://claude.ai)** (cuenta gratis con tu email o con Google; ⚠️ puede pedir un móvil, si no quieres darlo usa la de tu pareja): **Ajustes > Conectores > Descubrir**, busca **Figma** y pulsa **Conectar**.
3. Se abre Figma: inicia sesión y pulsa **Aceptar y permitir el acceso**.
4. **Duplica el Figma de Mint Scan** (botón 3 de la página de la clase) **con la misma cuenta de Figma que has conectado**: menú del nombre del archivo > **Duplicar** ⚠️ (el texto del menú puede variar un poco). Si lo duplicas con otra cuenta, Claude no podrá crear nada.
5. En tu copia, **Compartir > Copiar enlace** y pega ese enlace en Claude al principio de cada petición.

Claude te pedirá permiso en cada paso: pulsa **Permitir una vez** y mira qué va a tocar.

Un MCP es un enchufe para que la IA use otra herramienta. Como un USB-C: el mismo conector para muchos aparatos.

⚠️ Probado con Claude de pago y Figma gratis. **Con Claude gratis, sin probar.** Si no crea nada: comprueba que has pegado el enlace de **tu copia** y que la cuenta conectada es la dueña. Si sigue sin ir, únete a una pareja con Claude de pago o pídeme que lance tu prompt en pantalla.

⚠️ Claude gratis tiene pocos mensajes (Anthropic no da cifra; terceros estiman de 15 a 40 cada 5 horas). Prompts concretos y pocos; si se acaban, sigue con la cuenta de tu pareja.

## Cómo escribir tu prompt: las 5 C

Los prompts los escribes tú. Nada de copiar y pegar: es justo lo que vienes a practicar.

- **Cabeza:** quién eres y qué quieres.
- **Contexto:** para quién es, qué problema resuelve y con qué sistema de diseño.
- **Consultar:** que te pregunte lo que le falte antes de empezar.
- **Comprobar:** qué tiene que cumplir para estar bien. Lo miras tú en Figma.
- **Cortar:** una cosa cada vez. Nada de «rediséñalo todo».

### Antes de enviar, ¿tu prompt tiene…?

- [ ] El enlace de tu copia del Figma, al principio
- [ ] Quién es el usuario
- [ ] Qué quieres crear o qué dolor resuelves
- [ ] Que use los componentes y variables que ya hay: **Fila de campo**, **Insignia de confianza**, **Alerta**, **Botón** y **Chip de aviso**
- [ ] Qué tiene que cumplir para estar bien
- [ ] «Antes de empezar, pregúntame lo que necesites»
- [ ] Una sola cosa

⚠️ No le pidas capturas para comprobarlo: con Figma gratis tienes unas 20 lecturas al mes (crear no las gasta). Termina con «Sin capturas de comprobación».

### Ejemplo de forma, no para copiar

Para que veas cómo suena uno con las 5 C, sobre algo que no es ninguno de los dolores:

> *[enlace de mi copia]* Soy diseñador de producto y quiero el estado vacío de la lista de campos: lo que ve un técnico de ITV cuando la IA no ha podido leer ningún dato. Crea un solo frame nuevo al lado del Editor, con los componentes y variables que ya hay. Tiene que quedar claro qué ha pasado y qué puede hacer. Antes de empezar, pregúntame lo que necesites. Sin capturas de comprobación.

## Práctica 1: lo escribes tú

Pide a Claude que cree **una cosa pequeña** en tu copia. Ideas: una variante nueva de un componente, una pantalla con piezas que ya existen o un aviso nuevo. El estado vacío ya está pillado por el ejemplo.

Abre Figma y míralo. ¿Ha usado tus componentes o se ha inventado otros?

## Ronda 1: rediseña tu dolor

Escribe tu prompt con tu fila del encargo (documento 1):

- Tu **«Le duele…»** es lo que quieres resolver.
- Tu **«Sabremos que está resuelto si…»** es lo que tiene que cumplir.
- Pide **un solo frame nuevo** al lado del Editor, sin tocar el original.

Repasa la lista de arriba y envíalo.

Luego **retócalo a mano**: decides tú, no Claude. ¿Otro cambio? Uno cada vez: di en qué frame y qué cambia, y nada más.

## Tus datos

Claude: puedes impedir que entrene con tus chats en **Ajustes > Privacidad**.
Figma **entrena con tus archivos por defecto** en el plan gratis y en Professional (en Education, no). Por eso hoy solo usamos datos inventados.

## Si usas Claude Code

```
claude mcp add --transport http figma https://mcp.figma.com/mcp
```

Añade `--scope user` para tenerlo en todos tus proyectos y escribe `/mcp` para iniciar sesión en Figma.
