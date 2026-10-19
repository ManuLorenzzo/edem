# Guía · Conectar Figma con Claude

**Tú diseñas y decides. Claude te asiste. Make lo hace funcionar.**

Objetivo: conectar Claude con Figma y **ver que lo que escribís en Claude aparece en vuestro Figma**, usando vuestros componentes y variables. Después lo retocáis a mano. Claude también puede leer el archivo para revisarlo, pero eso es secundario. Basta una cuenta por pareja.

Datos verificados el 19 oct 2026 con una prueba real (Figma gratis y Claude de pago). Las herramientas cambian cada mes: si algo no coincide con la pantalla, avisad.

---

## Lo más fácil: pídeselo a tu IA

No hace falta saber instalar nada. Escríbele a tu IA: «Conéctate al MCP de Figma y guíame». Si tiene acceso a tu ordenador (Claude Code, Claude Desktop, Cowork), lo instala ella misma; en claude.ai te lleva paso a paso hasta el botón de conectar.

Si usas **Claude Code** y prefieres hacerlo tú, el comando oficial de Figma es:

```
claude mcp add --transport http figma https://mcp.figma.com/mcp
```

(Añade `--scope user` para tenerlo en todos tus proyectos. Luego escribe `/mcp` para iniciar sesión en Figma.)

Abajo tienes el camino manual en claude.ai, que es el que usaremos en clase. En resumen: cuenta de Claude, conectar Figma, **duplicar el Figma de Mint Scan con la misma cuenta que has conectado y pegar su enlace en Claude**, y pedir.

## Paso 1 · Cuenta de Claude gratis (2 minutos)

1. Entra en **claude.ai** y regístrate con tu email o con Google.
2. ⚠️ Puede pedir un número de móvil para verificar. Si no queréis darlo, usad la cuenta de vuestra pareja.
3. Al darte de alta te pregunta si tus conversaciones pueden usarse para entrenar. Puedes desactivarlo cuando quieras en **Ajustes > Privacidad**.

El plan gratuito incluye chat, artifacts (miniaplicaciones que se pueden publicar con un enlace), Claude Design y conectores. Tiene límites de uso bajos: escribid prompts concretos.

## Paso 2 · Conectar Figma (3 minutos)

1. En claude.ai, ve a **Ajustes > Conectores > Descubrir**.
2. Busca **Figma** (conector oficial, publicado por Figma) y pulsa **Conectar con Claude**.
3. Se abre Figma: inicia sesión y pulsa **Aceptar y permitir el acceso**. Pide lectura y escritura de tu cuenta.
4. Vuelve a Claude. Figma debe aparecer como conectado.

**Importante: la cuenta de Figma que conectáis tiene que tener acceso al archivo.** Por eso, en el paso 3, el Figma de Mint Scan se duplica con esa misma cuenta. Si lo duplicó tu pareja con la suya, o lo duplicas tú en la tuya, o tu pareja te lo comparte con permiso de edición. Si no, Claude no podrá crear nada en él.

**Permisos:** antes de usar cada herramienta, Claude pide permiso. Pulsad **Permitir una vez**: así veis qué va a tocar en vuestro Figma.

Por debajo esto es un **MCP**: un enchufe estándar para que una IA use otra herramienta. Como un USB-C: el mismo conector para muchos aparatos.

**Vuestros datos en Figma:** Figma **entrena su IA con vuestros archivos por defecto en los planes Starter (gratis) y Professional**. Lo puede apagar quien administra el equipo, en los ajustes del equipo. En Education no entrena. Por eso en clase solo usamos datos inventados. Fuente: help.figma.com/hc/en-us/articles/17725942479127

## Paso 3 · Duplica el Figma de Mint Scan y pega su enlace en Claude (1 minuto)

**Duplícalo con la misma cuenta de Figma que has conectado a Claude.** Si usas otra, Claude no podrá crear nada en tu copia.

1. Abrid el enlace del Figma de Mint Scan: https://www.figma.com/design/ogBGVM8Qvr7OKLsyEIQyzd
2. Duplicadlo en los borradores **de la cuenta que habéis conectado a Claude** (menú del nombre del archivo > **Duplicar**). ⚠️ El texto exacto del menú en castellano puede variar un poco.
3. En vuestra copia, **Compartir > Copiar enlace**.
4. **Pegad ese enlace en el chat de Claude**, al principio de cada petición.

Trae variables (colores de marca y de confianza, espaciados de 4 px) y componentes: **Fila de campo** (Normal, Seleccionada, Revisada, Vacía), **Insignia de confianza**, **Alerta**, **Botón** y **Chip de aviso**. Pedidle a Claude que los use.

## Paso 4 · Escribe en Claude, aparece en tu Figma (práctica 1)

**20 minutos, por parejas.** Le pedís a Claude que **cree** algo en vuestra copia usando los componentes y variables que ya existen, y lo veis aparecer en Figma.

### Cómo pedirlo: las 5 C

| C | Qué hacer |
|---|---|
| **Cabeza** | Di quién eres y qué quieres |
| **Contexto** | El usuario, el objetivo y tu sistema de diseño (los componentes y variables del archivo) |
| **Consultar** | «Antes de empezar, pregúntame lo que necesites» |
| **Comprobar** | **Dile qué tiene que cumplir; lo miras tú en Figma.** No le pidas capturas para comprobarlo: cada captura o consulta gasta lecturas, y con Figma gratis tenéis unas 20 al mes (escribir en Figma no las gasta). Por eso los ejemplos acaban en "Sin capturas de comprobación" |
| **Cortar** | Una petición concreta cada vez: una variante, un frame, un aviso. Nada de "rediséñalo todo" |

Y una cosa más: **Claude pide "Permitir una vez" en cada paso.** Aceptad y mirad qué va a tocar.

Ejemplos (pegad antes el enlace a vuestra copia):

**A · Una variante de un componente**
```
Crea en este archivo una variante nueva de la Fila de campo, "Con alerta pendiente": borde ámbar y un aviso corto debajo del valor, usando los componentes y variables que ya existen. Sin capturas de comprobación.
```

**B · Una pantalla nueva con instancias**
```
Crea en la página Editor un frame nuevo de 1440x900 llamado "Editor · todo revisado". Usa instancias de la Fila de campo en variante Revisada y un Botón primario "Imprimir". Solo componentes y variables que ya existen. Sin capturas de comprobación.
```

**C · Un estado vacío**
```
Crea un frame "Editor · sin campos" para cuando la IA no ha podido leer ningún campo del documento: un mensaje, una línea que explique qué hacer y un Botón primario "Volver a escanear". Usa los componentes y variables que ya existen. Sin capturas de comprobación.
```

**D · Un aviso nuevo**
```
Añade al componente Alerta una variante nueva para "Sin conexión con la impresora", con las variables de aviso y la misma estructura que las otras variantes. Sin capturas de comprobación.
```

Abrid Figma y comprobad vosotros qué ha creado. **Entregable de la pareja:** lo que ha creado (captura o enlace), **una cosa que hizo bien y otra que no** (¿usó vuestros componentes o dibujó copias? ¿respetó las variables?).

⚠️ Probado el 19 oct con Claude de pago y Figma gratis. **No está probado con Claude gratis.** Si en vuestra pareja no funciona, juntaos con una pareja que tenga Claude de pago o pedid al profesor que lance vuestro prompt en pantalla.

## Paso 5 · Leer y revisar (secundario)

Claude también puede **leer** un frame y revisarlo. Gasta lecturas (de 2 a 4 por "descríbeme esta pantalla"), así que haced **un único prompt de lectura** que lo pida todo. Pedid siempre sobre **un frame**: selecciónalo, clic derecho > **Copiar/Pegar como** > **Copiar enlace a la selección** (en inglés, *Copy/Paste as > Copy link to selection*).

```
[pega aquí el enlace al frame]

Eres un diseñador de producto sénior. Lee este frame de Figma una sola vez y dame, en un único mensaje:
1. Descripción: qué pantalla es, sus zonas y elementos principales y el recorrido del usuario, en 5 líneas.
2. Estilos: una tabla con elemento, color, tipografía, tamaño y espaciado que usa, y si está en el sistema de diseño (verde #4AB586, Inter, JetBrains Mono, base de 4 px, confianza alta #4AB586, media #E89672, baja #FF6961) o parece inventado.
3. Estados: qué estados faltan por diseñar (vacío, cargando, error, sin conexión, campo revisado, todo revisado...), una línea para cada uno.
Usa solo lo que leas del archivo. Si algo no lo puedes leer, dilo. No inventes nada.
```

Después, en el mismo chat y sin gastar lecturas, empezad con **"No vuelvas a leer el archivo: trabaja con lo que ya has leído."**

```
No vuelvas a leer el archivo: trabaja con lo que ya has leído.
El usuario es un técnico de ITV experto, con prisa, que revisa de 40 a 70 campos y desconfía de la IA.
¿Qué es lo primero que ve en esta pantalla? ¿Es lo que debería ver primero?
Señala 5 problemas de jerarquía visual, de más a menos grave, con una propuesta concreta para cada uno.
```

## Límites

| | Figma Starter (gratis) | Figma Education |
|---|---|---|
| Escribir por MCP (crear en Figma) | No gasta lecturas (gratis mientras esté en beta) | Igual |
| Leer por MCP | **Unas 20 lecturas al mes**; un "describe" gasta de 2 a 4 | **200 al día** (10 por minuto) |
| Figma Make | 500 créditos al mes, 150 al día | 3.000 al mes |
| ¿Entrena con tus archivos? | Sí, por defecto (lo apaga el admin del equipo) | No |

- **El otro freno son los mensajes de Claude gratis.** Anthropic no publica cifra; ⚠️ terceros estiman de 15 a 40 cada 5 horas. Crear en Figma encadena varias herramientas por petición: prompts concretos y pocos.
- Figma Make gasta créditos de Figma, no mensajes de Claude ni lecturas.

¿Qué plan tengo? En Figma, mira el nombre del plan del equipo en el menú de la cuenta.

## Si falla

Hay fallos conocidos (foro de Figma) y no son culpa vuestra. No perdáis más de 5 minutos.

- **No crea nada en Figma:** comprobad que habéis pegado el enlace a **vuestra copia** y que la cuenta de Figma conectada a Claude es la dueña de esa copia. Si sigue sin crear (sobre todo con Claude gratis), plan B: otra pareja con Claude de pago o el profesor en pantalla con vuestro prompt.
- **No lee el enlace:** comprobad que es el enlace a la selección (paso 5) y que **la cuenta de Figma conectada a Claude tiene acceso al archivo**.
- **No encuentra la herramienta:** pedídselo explícito ("usa el conector de Figma para crear esto en este archivo"). Si sigue, chat nuevo; si sigue, desconecta y vuelve a conectar Figma.
- **Se acaban las lecturas de Figma:** exportad el frame como PNG, arrastradlo al chat y usad el mismo prompt. Claude verá una imagen, no las capas: colores y medidas aproximados.
- **Se acaban los mensajes de Claude:** seguid con la cuenta de la pareja.
