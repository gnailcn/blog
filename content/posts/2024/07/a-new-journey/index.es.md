---
title: "Primer Post: Una Guía para Construir 'El Errante Recolector de Mareas'"
date: 2024-07-25T11:00:00+08:00
categories: ["hugo"]
tags: ["hugo"]
summary: "Este no es solo el primer post en este sitio, sino también un documento vivo sobre cómo añadir nuevas entradas e imágenes: un plano para nuestro futuro flujo de trabajo creativo."
draft: false
---

Hola, mi yo del futuro, y a cualquier amigo que pueda llegar a visitar este lugar.

Bienvenidos al comienzo de "El Errante Recolector de Mareas". Este espacio está concebido como una cesta para guardar las "conchas" y "estrellas" que recojo a orillas de la marea del conocimiento y la información. Hoy, coloco la primera concha cuidadosamente seleccionada: una guía sobre cómo crear contenido aquí.

Este post sirve tanto de recuerdo como de manual de operaciones, asegurando que cada futura creación sea clara y eficiente.

## I. El Punto de Partida: Un Único Comando

No creamos archivos manualmente. En su lugar, usamos la elegante herramienta de línea de comandos de HUGO. Es como una varita mágica que nos prepara todo.

Abre tu terminal, navega a la raíz del blog y recita el hechizo:

```bash
# Formato: hugo new tipo-de-contenido/AAAA/MM/tu-slug-del-post/index.idioma.md
hugo new posts/2024/07/a-new-journey/index.es.md
```

Este comando realiza un poco de magia:

1.  Crea una carpeta llamada `a-new-journey` dentro del directorio `content/posts/2024/07/`.
2.  Dentro de esa carpeta, crea un archivo `index.es.md`.
3.  Rellena automáticamente este archivo con "información de identidad" (el Front Matter), incluyendo el título, la fecha y una bandera crucial: `draft: true`. Esta bandera lo marca como un borrador, visible en las vistas previas locales pero ignorado durante el despliegue final, lo cual es muy seguro.

Cuando hayamos terminado de escribir y estemos listos para que el mundo lo vea, simplemente cambiamos `draft: true` a `draft: false`.

## II. Dándole Alma: Palabras e Imágenes

Un artículo completo se compone tanto de texto como de imágenes. En nuestra estructura bien diseñada, gestionarlos se vuelve increíblemente simple.

### 1. Palabras

Debajo de la "información de identidad" del archivo es donde dejamos fluir nuestras palabras. Sigue la sintaxis estándar de Markdown: concisa y potente.

### 2. Imágenes: El Fin del Caos

Esta es la parte más hermosa de nuestro flujo de trabajo. **Cada artículo tiene su propia carpeta dedicada**, ¡lo que significa que todas las imágenes utilizadas en el artículo pueden almacenarse junto al propio artículo!

Supongamos que estamos escribiendo este post `a-new-journey`. Su estructura de directorios se ve así:

```
content/
└── posts/
    └── 2024/
        └── 07/
            └── a-new-journey/          <-- La carpeta dedicada del artículo
                ├── index.es.md         <-- El archivo del artículo en sí
                └── journey-start.jpg   <-- ¡Su imagen compañera!
```

**¿Cómo se hace referencia a esta imagen?**

En tu archivo `index.es.md`, solo necesitas escribir lo siguiente, sin ninguna ruta complicada:

```markdown
![El Comienzo del Viaje](journey-start.jpg)
```

![El Comienzo del Viaje](journey-start.jpg)

¡Así de simple! La imagen y el texto están elegantemente "empaquetados" juntos, haciendo que la migración, la copia de seguridad y la gestión sean una experiencia libre de preocupaciones.

## III. La "Tarjeta de Identidad" del Artículo: Front Matter

La zona en la parte superior de cada artículo, envuelta en `---`, son sus metadatos. Determina cómo se clasifica y se muestra el artículo.

-   **`title`**: El título del artículo.
-   **`date`**: La fecha de publicación, que determina su posición en los archivos.
-   **`categories`**: La categoría, generalmente una única clasificación amplia como `["Notas Técnicas"]` o `["Reflexiones de Vida"]`.
-   **`tags`**: Las etiquetas, que pueden ser múltiples y se utilizan para una indexación más granular, como `["Go", "Web", "Optimización de Rendimiento"]`.
-   **`summary`**: Un breve resumen que se mostrará en la página de lista de artículos.
-   **`draft`**: `false` significa que el artículo está publicado; `true` significa que es un borrador.

Rellenar cuidadosamente esta información mantendrá nuestra base de conocimientos limpia y organizada.

## Conclusión

El proceso creativo debe ser un placer, no una carga.

Comenzar el viaje con `hugo new`, colocar palabras e imágenes en su carpeta dedicada y, finalmente, quitarle el polvo a `draft`. Este es todo el secreto para registrar cada descubrimiento aquí en "El Errante Recolector de Mareas".

Que esta pequeña cesta se llene cada día más.