# Matriz · Para esta tarea de diseño, esta IA, por esto

Dos familias:

- **Generalistas** (Claude, ChatGPT, Gemini): para todo vuestro día a día, y también diseñan.
- **Especialistas de diseño** (Figma Make, Stitch, Framer, v0): solo diseñan y prototipan, dentro del flujo del oficio. Figma Make es la que os encontraréis en las empresas.

Para cada tarea, primero: **¿generalista o especialista?** Y para decidir entre candidatas, cuatro preguntas:

- **Valor**: ¿me ahorra trabajo o solo me lo cambia de sitio?
- **Datos**: ¿lo subiría si mi cliente estuviera mirando?
- **Riesgos**: ¿qué pasa si se equivoca y nadie lo revisa?
- **Viabilidad**: ¿me la puedo permitir cada semana, no solo para probarla?

En la matriz, «Porque…» es el valor, y **«¿Qué me preocupa?»** junta datos, riesgos y viabilidad: lo que os haría dudar antes de usarla.

Recordad: **motor ≠ herramienta**. Elegís la herramienta por la tarea; el motor de debajo importa menos de lo que parece.

---

## Vuestra matriz

| Quiero… | Usaría… | Porque… | ¿Qué me preocupa? |
|---|---|---|---|
| **Rediseñar una pantalla** | | | |
| **Prototipo navegable** | | | |
| **Iterar con un cambio** | | | |
| **Revisar antes de producción** | | | |
| *(una tarea vuestra)* | | | |

---

## Versión de referencia (Manu, octubre 2026)

Datos de planes y límites verificados el 19 oct 2026. Cambian cada mes: comprobadlos antes de decidir.

| Quiero… | Usaría… | Porque… | ¿Qué me preocupa? |
|---|---|---|---|
| **Rediseñar una pantalla** | Claude conectado a Figma, que crea en tu archivo con tus componentes y variables; tú lo retocas y decides. Para explorar fuera de Figma: Claude Design o Google Stitch | Más alternativas en menos tiempo, dentro de tu propio archivo y sin perder el control del diseño | Que se aleje de tu sistema de diseño o dibuje copias en vez de usar tus componentes. Que parezca terminado y no lo esté. Es beta y gasta muchos mensajes de Claude: prompts concretos. Probado con Claude de pago; ⚠️ con Claude gratis, sin probar. Claude Design no exporta a Figma; Stitch sí |
| **Prototipo navegable** | Figma Make. Plan B: artifact de Claude. Plan C: prototipo de Figma de siempre | Parte de tu frame y genera algo que funciona de verdad: estado, datos y casos raros | Estados que faltan, poca fidelidad al frame: revisarlo con la checklist. Hay que adjuntar el frame (pegar la URL no sirve). Un diseño adjunto cuesta unos 75 créditos o más: con Starter (150 al día, 500 al mes) salen unos 2 prompts al día; Education, 3.000 al mes. Modelo por defecto. Publicar en Starter obliga a hacerlo público en la Community. Figma entrena con tus archivos por defecto en Starter y Professional |
| **Iterar con un cambio** | Figma Make con los créditos de la pareja, o Claude sobre el artifact | Añadir un requisito sin rehacer desde cero | Que rehaga en vez de añadir y rompa lo que funcionaba. Preparar el cambio con Claude antes (no gasta créditos de Make) y lanzarlo en un único prompt |
| **Revisar antes de producción** | Claude en una conversación nueva, con el código o capturas (uno escribe, otro revisa) y la checklist al lado | Una revisión con las cinco preguntas en minutos y una lista de lo que le falta para ser una app de verdad | Hallazgos inventados: pedir "Demuéstralo". Contraste medido en una captura comprimida: comprobarlo en WebAIM o con Stark. Pasarle solo código o capturas sin datos reales y desactivar el entrenamiento en Ajustes > Privacidad. Por el conector de Figma, solo si tenéis Education (Starter: unas 20 lecturas al mes) |

### Otras tareas de vuestro día a día

| Quiero… | Usaría… | Porque… | ¿Qué me preocupa? |
|---|---|---|---|
| **Revisar un diseño en Figma** | Claude con el conector de Figma (MCP) | Lee capas, estilos y textos reales: revisión con datos, no a ojo | Que invente hallazgos: pedir "Demuéstralo". Starter: unas 20 lecturas al mes y un "describe" gasta de 2 a 4, así que un único prompt de lectura. Education: 200 al día. La cuenta de Figma conectada tiene que tener acceso al archivo |
| **Research de mercado y competencia** | Deep Research de Gemini (o de ChatGPT) | Un informe con fuentes en minutos, en vez de una tarde de búsquedas | Fuentes flojas o mal citadas: abrir y comprobar al menos 3. Solo información pública, nada de datos de clientes. Gemini lo incluye gratis; ChatGPT Free, limitado; en Claude gratis no está |
| **Sintetizar entrevistas con usuarios** | Claude chat, con un Project por estudio | Patrones, citas y dolores agrupados a partir de muchas notas | Datos personales: **anonimizar antes** y desactivar el entrenamiento en Ajustes > Privacidad. Citas inventadas o mezcladas: pedir citas literales y comprobarlas. Gratis, hasta 5 Projects, límites de uso bajos |
| **Documentar para desarrollo** | Claude con el conector de Figma (MCP) | Lista de componentes, variables y estados a partir del archivo | Documentación que no coincide con el diseño final: revisarla antes de entregar. Mismos límites de lectura que «Revisar un diseño en Figma» |

**Lo que no está en la matriz a propósito:** imagen y vídeo con IA (otra sesión) y "la IA que lo hace todo". Si una herramienta promete todas las filas, desconfía.
