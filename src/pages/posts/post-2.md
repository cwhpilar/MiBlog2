---

title: "Por qué mi nueva web con Astro vuela"
pubDate: 2026-07-01
description: "Analizo las claves técnicas que hacen de Astro el framework ideal para el rendimiento web."
author: "Tu Nombre"
tags: ["astro", "rendimiento", "javascript", "jamstack"]
---

# El secreto detrás de la velocidad de Astro

En mi publicación anterior compartí la alegría de lanzar esta web. Hoy quiero ponerme un poco más técnico y explicar la verdadera razón por la que decidí usar **Astro**: el rendimiento.

Si vienes de frameworks tradicionales como Next.js o Nuxt, la filosofía de Astro te cambiará la forma de pensar.

## Las 3 claves del rendimiento en Astro

* **Zero JavaScript por defecto**: Astro renderiza todo a HTML estático en el servidor.
* **Islas de interactividad**: El código JavaScript solo se descarga para los componentes dinámicos.
* **Carga perezosa inteligente**: Puedes decidir exactamente cuándo se hidrata un componente en pantalla.

## Comparativa visual: Frameworks tradicionales vs Astro

En un framework de Single Page Application (SPA) convencional, el navegador recibe un archivo HTML vacío y un bloque enorme de JavaScript que debe procesar antes de mostrar algo. 

Con Astro, el flujo es inverso:

1. El usuario solicita la página.
2. El servidor envía HTML puro y CSS ultra ligero.
3. La página es interactiva de inmediato.

## Un ejemplo de "Isla de Astro"

Para los elementos estáticos (como este texto), Astro no envía scripts. Pero si quisiera añadir un botón de "Me gusta" interactivo usando React, solo tengo que hacer esto:

```astro
---
import BotonMeGusta from '../components/BotonMeGusta.jsx';
---
<!-- Este componente se hidratará solo cuando sea visible en pantalla -->
<BotonMeGusta client:visible />
```

La directiva `client:visible` es pura magia. El JavaScript de ese botón no se descargará hasta que el usuario haga scroll y llegue a él.

## Próximos pasos

En el siguiente artículo compartiré las métricas de **Lighthouse** de esta web para demostrar con números reales cómo este enfoque impacta positivamente en el SEO.

¡Nos vemos en la próxima!

***

*¿Has probado la arquitectura de islas? Cuéntame tu experiencia.*
