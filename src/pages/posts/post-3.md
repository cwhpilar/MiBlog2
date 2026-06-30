---

title: "Consiguiendo un 100/100 en Lighthouse con Astro"
pubDate: 2026-07-02
description: "Analizo las métricas de rendimiento y SEO de mi nueva web y cómo Astro facilita una puntuación perfecta."
author: "Tu Nombre"
tags: ["astro", "seo", "lighthouse", "optimizacion"]
---

# Pasando el test de velocidad: Mis resultados en Lighthouse

Después de lanzar la web y entender la teoría de la arquitectura de islas, llegó el momento de la verdad. Sometí este sitio a las pruebas de **Google Lighthouse** y las herramientas de **PageSpeed Insights**.

Los resultados confirman que la obsesión de Astro por el HTML puro da sus frutos.

## El veredicto de las métricas

* **Rendimiento (Performance)**: 100/100
* **Accesibilidad (Accessibility)**: 100/100
* **Buenas Prácticas (Best Practices)**: 100/100
* **SEO**: 100/100

## ¿Cómo ayuda Astro a conseguir estos números?

Conseguir una puntuación perfecta en otros entornos suele requerir horas de optimización manual. Con Astro, viene integrado desde el primer minuto gracias a tres factores clave:

* **Optimización de imágenes integrada**: El componente `<Image />` de Astro comprime, redimensiona y convierte las imágenes a formatos modernos como WebP automáticamente.
* **Fuentes optimizadas**: La carga de tipografías no bloquea el renderizado de la página, evitando el parpadeo de texto (FOUT).
* **CSS crítico en línea**: Astro inyecta automáticamente solo el CSS que la página necesita, reduciendo el tiempo de carga inicial.

## Mi configuración para el éxito

Para lograr el 100% en SEO, añadí un par de integraciones oficiales del ecosistema de Astro que son imprescindibles para cualquier proyecto:

```bash
# Instalación del generador de sitemap automático
npx astro add sitemap
```

Esto genera el archivo `sitemap-index.xml` en cada despliegue, asegurando que los motores de búsqueda indexen todo el contenido de inmediato.

## Conclusión

Astro demuestra que no hace falta sacrificar la experiencia de desarrollo para obtener una web rápida. Puedes escribir componentes modernos y estructurados, mientras el usuario final recibe una página que carga de forma instantánea.

***

*¿Qué puntuación tienen tus proyectos actuales en Lighthouse? Si quieres mejorarla, te leo en los comentarios.*
