# Qué es cada cosa

Chuleta para no mezclar las piezas de la IA que usaréis en vuestro trabajo.

| Pieza | Qué es | Cuándo actúa | Ejemplo |
|---|---|---|---|
| **Prompt** | Lo que le pides ahora | Una vez | «Describe esta pantalla y dime qué estados faltan» |
| **Proyecto, Gem o GPT** | Contexto fijo que siempre está presente | Siempre, en ese espacio | Un proyecto de Claude con el brief y el sistema de diseño |
| **Skill** | Un documento con el procedimiento de «cómo se hace aquí» | Solo cuando la tarea lo pide | «Revisión de pantallas según nuestro sistema de diseño» |
| **MCP** | Las llaves para que la IA toque una herramienta | Cuando la IA la necesita | El conector de Figma |
| **Plugin** | Un paquete de skills y MCP que se instala de una vez | Desde que lo instalas | Los plugins de ChatGPT que sustituyen a los GPTs |
| **Agente** | Quien lo orquesta todo: decide el siguiente paso, actúa y comprueba | Él decide | Claude revisando tu Figma con tu skill |
| **Arnés (harness)** | El programa que envuelve al motor y le da memoria, permisos, herramientas y el bucle | Siempre, es «la herramienta» | claude.ai, Claude Code, Figma Make |
| **Motor (modelo)** | El que piensa | Dentro de todo lo anterior | Claude, Gemini, GPT |

**Anatomía de un agente:** motor (piensa) + skill (sabe cómo se hace aquí) + MCP (puede tocar tus herramientas) + bucle (decide, actúa, comprueba, repite), todo dentro de un arnés.

**La pregunta para distinguir chatbot, asistente, automatización y agente:** ¿quién decide el siguiente paso?
