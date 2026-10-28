# AgroCampo Huila - Landing Page

Este proyecto es una página web responsive para una tienda de insumos agrícolas en el departamento del Huila. Fue desarrollada como parte del Seminario de Gestión de Software Ágil, cumpliendo con los lineamientos de diseño UX/UI, accesibilidad y la regla de color 60-30-10.

**Tecnologías usadas:** HTML5, Tailwind CSS v4 (Play CDN) y JavaScript puro (Vanilla JS).

## Bitácora de Prompts (Fase de Generación con IA)

A continuación se documentan las 5 iteraciones principales realizadas con inteligencia artificial para corregir y mejorar el código generado inicialmente:

| # | PROMPT DE AJUSTE ENVIADO | PROBLEMA QUE BUSCABA RESOLVER | RESULTADO OBTENIDO | ¿FUNCIONÓ? |
|---|---|---|---|---|
| **1** | *"El menú hamburguesa en celular no hace nada, haz que se abra y cierre usando JavaScript puro sin alterar el HTML base."* | El menú de navegación móvil no respondía al hacer clic. | Se añadió la lógica con `addEventListener('click')` al botón `menu-toggle`. | Sí |
| **2** | *"El modo oscuro funciona, pero los campos del formulario se quedan blancos y no se leen. Ajusta las clases de los input."* | Contraste deficiente en los campos del formulario durante el tema oscuro. | Se agregaron las clases `dark:bg-slate-900` y bordes oscuros en los inputs. | Sí |
| **3** | *"Modifica el acordeón de preguntas frecuentes para que solo permita tener una pregunta abierta a la vez."* | Se podían desplegar todas las respuestas simultáneamente, rompiendo el diseño. | Se configuró el JS para ocultar los paneles abiertos al hacer clic en uno nuevo. | Sí |
| **4** | *"El mensaje verde de éxito al enviar el formulario se queda estático en pantalla. Haz que desaparezca a los 4 segundos."* | El mensaje tipo Toast no tenía temporizador de cierre. | Se implementó un `setTimeout` de 4000ms en la función `showToast`. | Sí |
| **5** | *"Añade un texto dinámico arriba del catálogo que me diga cuántos productos he seleccionado con los botones de 'Añadir'."* | El usuario no tenía retroalimentación visual de los productos seleccionados para cotizar. | Se creó el panel `quote-selection` gestionado mediante un `Set` en JavaScript. | Sí |

## Cambios Manuales Realizados (Fase 5)
Para demostrar comprensión del código, se realizaron 3 cambios sin asistencia de IA:
1. Modificación de la variable `--color-ambar` en la directiva `@theme`.
2. Cambio del tiempo del Toast en JavaScript de 4000 a 6000 milisegundos.
3. Personalización manual del texto de éxito en la función `showToast`.# AgroCampoHuila
