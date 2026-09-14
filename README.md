# Sitio Web Estatico de Recetas

Este sitio web estatico fue desarrollado aplicando técnicas de ingeniería de prompts sobre el modelo de inteligencia artificial ChatGPT.

---

## Prompt Utilizado


```text
Actúa como un desarrollador web experto en HTML5 y CSS3. Necesito que generes el código para un sitio web estático de recetas de cocina siguiendo estrictamente las siguientes reglas y especificaciones:

1. RESTRICCIONES TÉCNICAS ESTRICTAS:
   - Solo debes utilizar HTML5 y CSS3 puro. 
   - Queda totalmente prohibido el uso de JavaScript o cualquier tipo de script.
   - Todo el código CSS debe ir en un archivo independiente llamado `estilosIA.css`. Proporciona el código HTML y CSS en bloques separados.

2. ESTRUCTURA Y NAVEGACIÓN (HTML):
   - Incluye una barra de navegación (navbar) con tres enlaces principales:
     1. Información de contacto (que dirija a una sección con un formulario simple de contacto).
     2. Información de quien mantiene el sitio (sección "Sobre mí" / mantenedor).
     3. Catálogo de recetas agrupadas en las categorías: "salado" y "dulce".

3. INTERACCIÓN ESTÁTICA Y FILTRADO (CSS PURO):
   - Implementa un sistema de selección por categoría ("salado" y "dulce") mediante radio buttons (`<input type="radio">`) o una lista desplegable/control estático usando CSS puro (técnica de radio buttons + pseudo-clase `:checked`), sin nada de JS.
   - Al seleccionar una categoría, deben filtrarse u ocultarse/mostrarse dinámicamente en el área central las recetas correspondientes de forma 100% estática.

4. DISEÑO DE TARJETAS DE RECETAS:
   - En la zona central, muestra recuadros (tarjetas) para cada receta.
   - Cada tarjeta debe contar con un borde y un color de relleno/background armónicos bien definidos visualmente.
   - Cada recuadro debe contener:
     * Nombre de la receta.
     * Una imagen representativa.
     * Un enlace para descargar la receta en PDF.

5. ARCHIVOS Y ESTRUCTURA DE RUTAS:
   - Debes incluir al menos 3 recetas por cada categoría (mínimo 6 recetas en total: receta1 a receta6).
   - Las imágenes deben apuntar a la carpeta `imágenes/` con formato PNG (ejemplo: `imágenes/receta1.png`).
   - Los archivos PDF deben apuntar a la carpeta `recetarios/` (ejemplo: `recetarios/receta1.pdf`).

6. DISEÑO RESPONSIVO Y ESTILOS:
   - El sitio debe ser completamente responsivo (adaptable a móviles, tablets y escritorio) mediante Media Queries en CSS.
   - Aplica una paleta de colores limpia, profesional y moderna.

---
```
## Criterios de Ingeniería de Prompts Aplicados

El prompt se diseñó contemplando cuatro aspectos clave:

* **Asignación de Rol (Persona):** Se definió a la IA como "desarrollador web experto". Esto ajusta sus respuestas para que aplique buenas prácticas del sector y mantenga un estándar profesional.
* **Delimitación de Restricciones Estrictas:** Se aislaron explícitamente las limitaciones del proyecto (descarte total de JavaScript, uso exclusivo de HTML/CSS) y el nombre exacto del archivo de estilos (`estilosIA.css`). Establecer límites claros evita que el modelo incluya librerías externas o archivos no solicitados.
* **Estructura Jerárquica:** El prompt se organizó en bloques temáticos y numerados. Esta división facilita la lectura por parte del modelo y disminuye las probabilidades de que se omitan detalles secundarios.
* **Arquitectura de Archivos y Rutas:** Se indicaron con precisión la cantidad de recetas (mínimo 6), los nombres de las carpetas (`imágenes/`, `recetarios/`) y sus respectivas extensiones (`.png`, `.pdf`) para asegurar la compatibilidad con el proyecto local.

---

## Demo del Sitio Web

Ingresar en el siguiente enlace:

[Web estatica generada por Gemini](https://thnicolas.github.io/Sitio1/)