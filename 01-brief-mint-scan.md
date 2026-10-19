# Brief · Mint Scan: revisar la tarjeta que propone la IA

Caso real, datos inventados. Todo vehículo, bastidor, estación y persona de este brief es ficticio.

---

## Qué es Mint Scan (aunque no sepas qué pasa dentro de una ITV)

Cuando un coche se matricula en España o necesita un duplicado, la estación ITV emite su **Tarjeta ITV**: un documento oficial con decenas de campos técnicos (marca, bastidor, masas, medidas, motor, homologación). Hoy, en muchas estaciones, un técnico copia esos campos a mano desde la documentación del fabricante, a veces en otro idioma.

**Mint Scan** lee esos documentos con IA, **propone la tarjeta ya rellena** con una confianza por campo y avisos de incoherencias, y el técnico revisa, corrige e imprime sobre el papel oficial.

Lo usan unas **150 estaciones** y genera **más de 5.000 tarjetas al mes**.

## El usuario

**Técnico de la oficina técnica de una ITV.**

- Experto: conoce la normativa mejor que nadie en la sala.
- Desconfiado de la "caja negra": necesita ver **de dónde sale cada dato** antes de firmarlo.
- Trabaja con volumen, todo el día, a menudo con el cliente esperando.
- Escritorio, pantallas de 1280 px o más. No usa el móvil para esto.

Vocabulario del producto: **Borrador** es la tarjeta editable; al imprimirla pasa a **Tarjeta generada**.

## La tarea que vais a diseñar

El flujo completo es: **panel de trabajo > editor > generar > imprimir**. Vosotros diseñáis estos tramos:

1. **Revisar** (el editor, a fondo): la tarjeta que propone la IA, con el documento original a un lado y la lista de campos al otro; cada campo con su confianza (alta, media, baja), de qué documento sale y sus alertas.
2. **Imprimir** (la pantalla de éxito): vista previa y confirmación de que la tarjeta se ha generado e impreso.
3. *Opcional:* **Generar**, la revisión previa con errores y avisos, número de tarjeta e impresora.

## Lo que le duele hoy

Dolores reales del producto. Cómo se arreglan en pantalla lo decidís vosotros: sois los expertos en diseño.

| Le duele… | Sabremos que está resuelto si… |
|---|---|
| Tiene **70 datos** y no sabe cuáles mirar primero | En **5 segundos** sabe qué le falta |
| Pincha un dato y no ve **de dónde sale** en el documento | Sabe de dónde sale cada dato sin buscarlo |
| Los **colores no significan lo mismo** en todas las pantallas | Un color quiere decir lo mismo en todas partes |
| Le salta un aviso y **no puede aceptarlo ni descartarlo**: solo le lleva al campo | Puede aceptar, corregir o descartar cada aviso |
| Ve un **98 % en verde** y deja de mirar (es una confianza técnica, no una precisión medida) | Un número alto no le hace dejar de mirar |

## Vuestro dolor: uno por pareja

Cada pareja rediseña **un solo dolor** de la tabla de arriba, el de su número de pareja (el profesor os numera al empezar la clase):

| Pareja | Dolor |
|---|---|
| 1 | Tiene 70 datos y no sabe cuáles mirar primero |
| 2 | Pincha un dato y no ve de dónde sale en el documento |
| 3 | Los colores no significan lo mismo en todas las pantallas |
| 4 | Le salta un aviso y no puede aceptarlo ni descartarlo |
| 5 | Ve un 98 % en verde y deja de mirar |
| 6 (si la hay) | También el 5: dos enfoques distintos del mismo dolor |

Entre todas cubrís la pantalla entera. Ir a fondo con uno es mejor que tocar cinco por encima: vuestro criterio de éxito es la columna «Sabremos que está resuelto si…» de vuestra fila.

Trabajáis sobre **vuestra copia del Figma de Mint Scan, página Editor**.

## El reto de diseño

> **¿Cómo se diseña la revisión humana de lo que propone una IA?**

Que el técnico vaya rápido sin fiarse a ciegas: que sepa qué mirar primero, de dónde sale cada dato, qué le queda y cuándo puede imprimir con tranquilidad.

## Restricciones

- **App de escritorio en Windows**, pantallas de 1280 px o más. Nada de móvil.
- **Usuarios intensivos**: trabajan todo el día con la misma pantalla y usan atajos de teclado.
- **Papel oficial preimpreso**: la tarjeta se imprime sobre un formulario oficial, no sobre papel en blanco.
- **De 40 a 70 campos reales** por tarjeta. La tabla de abajo es solo una muestra.
- **Flujo fijo**: panel de trabajo, editor, generar, imprimir.
- **No se toca el sistema de diseño de Mint**: verde `#4AB586`, Inter para la interfaz, JetBrains Mono para códigos y datos, base de 4 px. Confianza alta `#4AB586`, media `#E89672`, baja `#FF6961`. Lo podéis criticar en el informe, pero no cambiarlo en el prototipo.

## Alcance

- **Un frame, un dolor**: el editor de revisión con vuestro dolor resuelto. No tiene que quedar perfecto. La pantalla de éxito no la dibujáis: la describe el prompt de Make. La de generar (revisión previa), fuera.
- **Prototipo que funciona**, hecho con Figma Make a partir de vuestro frame: se hace clic, se pasa de una pantalla a otra y los datos cambian.
- Partís del Figma de partida (enlace en la slide), que ya usa el sistema de diseño de Mint Scan.
- El rediseño se centra en **vuestro dolor**; lo demás de la pantalla puede quedarse como está.

## Datos de ejemplo (ficticios)

Vehículo: **Marca Ejemplo Modelo X**, turismo. Documento de origen: un COC (certificado de conformidad europeo) de 4 páginas.

| Código | Campo | Valor propuesto | Confianza | Sale de | Alerta |
|---|---|---|---|---|---|
| D.1 | Marca | Marca Ejemplo | 99 % | COC, pág. 1 | |
| D.2 | Tipo / Variante / Versión | MX1 / A / 01 | 91 % | COC, pág. 1 | |
| D.3 | Denominación comercial | Modelo X | 95 % | COC, pág. 1 | |
| E | Bastidor | ZZZ00000000000001 | 98 % | COC, pág. 1 | |
| J | Categoría | M1 | 97 % | COC, pág. 1 | |
| K | Contraseña de homologación | e9\*0000/0000\*0000 | 72 % | COC, pág. 1 | Formato dudoso |
| F.1 | Masa máxima técnica | 2.100 kg | 64 % | COC, pág. 2 | No coincide con el COC |
| F.2 | Masa máxima en servicio | 2.100 kg | 80 % | COC, pág. 2 | |
| G | Masa en orden de marcha | 1.450 kg | 88 % | COC, pág. 2 | |
| L | Número de ejes | 2 | 99 % | COC, pág. 2 | |
| P.1 | Cilindrada | 1.598 cm³ | 93 % | COC, pág. 3 | |
| P.2 | Potencia neta máxima | 85 kW | 90 % | COC, pág. 3 | |
| P.3 | Combustible | Gasolina | 96 % | COC, pág. 3 | |
| S.1 | Plazas sentadas | 5 | 99 % | COC, pág. 3 | |
| V.7 | Emisiones de CO2 | 142 g/km | 58 % | COC, pág. 4 | Valor fuera de rango habitual |
| (sin código) | Neumáticos | 205/55 R16 | 0 % | | Campo vacío |

Las tres alertas son a propósito. Son 16 campos de muestra: la tarjeta real tiene de 40 a 70. Los códigos son orientativos: para el ejercicio da igual que no sean exactos.

---

## Cómo va la práctica 2: tres rondas cortas

Tres rondas de unos 15 minutos. Cada una empieza con el profesor en pantalla, sigue con vosotros trabajando y acaba con una parada de 3 minutos para ver resultados. Todo en vuestra copia del Figma de Mint Scan, página Editor, y sobre vuestro dolor.

**Solo se proyecta desde el portátil del profesor.** Por eso lo que hacéis va desde el principio a **vuestro hueco del tablero de la clase** (el enlace está en la portada del kit, `README.md`): en las paradas, el profesor abre desde ahí lo que habéis pegado.

| Ronda | El profesor arranca | Vosotros (unos 10 min) | Parada (3 min) |
|---|---|---|---|
| **1 · Rediséñalo con Claude** | Pega en pantalla el prompt del kit con un dolor y lo envía | Pegáis el prompt (`03-vias-prototipo.md`, ronda 1) con vuestro dolor: Claude crea el rediseño en vuestro Figma con el conector y lo retocáis a mano. **Un frame, un dolor. No tiene que quedar perfecto.** Antes de la parada, pegad en vuestro hueco del tablero el **enlace de vuestra copia del Figma** (Compartir, «Cualquiera con el enlace», permiso **Ver**) | El profesor abre dos desde el tablero: ¿qué ha hecho bien Claude y qué no? |
| **2 · Hazlo funcionar en Make** | Explica cómo se usa Figma Make y lo hace con vosotros: pega su frame en Make a la vez | Copiáis vuestro frame, lo pegáis en el chat de Make con **un solo prompt** del kit (Make tarda unos 3 minutos) y lo probáis con clics. **En cuanto funcione, publicadlo** y pegad el **enlace del prototipo** en vuestro hueco | ¿A quién le funciona? El profesor abre uno desde el tablero. Si Make falla, prototipo de Figma de siempre |
| **3 · El cliente cambia de idea** | Os cuenta un cambio del cliente | Se lo pedís a Make **en el mismo chat**, no en Claude. Cambiad solo lo necesario. Después, **volved a publicar**: el enlace es el mismo, no hace falta pegarlo otra vez | El profesor abre uno desde el tablero: ¿ha roto algo que antes funcionaba? |

Claude, con el conector, solo diseña en Figma. Figma Make es otra herramienta, con su propio chat, que convierte vuestro frame en una app que funciona. Por eso, después de Make, los cambios se piden en el chat de Make.

El cambio de la ronda 3 lo veréis en pantalla. Es el mismo para todas las parejas: cada una lo aplica a su dolor.

Cómo compartir la copia del Figma y cómo publicar en Make: `03-vias-prototipo.md`, «Cómo publicar y compartir». Con Figma gratis, publicar en Make obliga a dejarlo público en la Community de Figma: no pasa nada, los datos son inventados.

## Qué entregáis y dónde

**Al acabar la ronda 3 (3 minutos):**

1. **Publicad la versión final** de vuestro prototipo de Figma Make.
2. **Abrid vuestro enlace en una ventana de incógnito**: si se ve sin iniciar sesión, está bien. Es el que usará la pareja que os revise.
3. La pareja que os revise tiene el enlace de vuestro Figma de la ronda 1 para comparar con el prototipo.
4. ¿El tablero no va? Mandad número de pareja, dolor y los dos enlaces por email al profesor (dirección en la slide de entrega).

**Práctica 3: revisáis el prototipo de otra pareja.** La 1 revisa el de la 2, la 2 el de la 3… y la última el de la 1. Sacáis su enlace del tablero y a intentar romperlo, con el prompt de revisión (`05`) y la checklist (`04`). El informe (`06`) es sobre el prototipo que revisáis. Antes de la puesta en común, dejad en su hueco del tablero un post-it con vuestros tres hallazgos principales.

**Puesta en común (90 segundos por pareja, en orden de dolor del 1 al 5; el profesor proyecta vuestro hueco del tablero):**

1. Vuestro dolor y cómo lo habéis resuelto.
2. Lo que encontró la pareja que os revisó.
3. Lo que más le falta para ser una app de verdad.

La pregunta de la puesta en común no es de diseño: **¿le resuelve el dolor al técnico?**

**Después de clase (opcional):** mandad el informe terminado por email al profesor.
