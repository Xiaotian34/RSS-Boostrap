# Lector de Noticias ATOM/RSS

Un lector de feeds ATOM y RSS moderno y fácil de usar, creado con HTML, CSS y JavaScript puro. Esta aplicación web te permite leer, buscar y guardar como favoritas noticias de múltiples fuentes.

## Características

- **Soporte para formatos ATOM y RSS**: Compatible con ambos formatos de sindicación.
- **Interfaz minimalista**: Diseño limpio con colores fríos para una agradable experiencia de lectura.
- **Visualización en tarjetas**: Las noticias se muestran en tarjetas con imágenes y resúmenes.
- **Paginación**: Muestra 10 noticias por página con navegación intuitiva.
- **Búsqueda**: Filtrado rápido de noticias por texto en título, resumen, autor o categoría.
- **Favoritos**: Guarda tus noticias favoritas para leerlas más tarde.
- **Soporte CORS**: Incluye un proxy para superar limitaciones de origen cruzado.
- **Detección de imágenes**: Extrae imágenes de diferentes partes de los feeds para una mejor visualización.
- **Responsive**: Diseño adaptable a diferentes tamaños de pantalla.

## Cómo usar

1. **Añadir un feed**: Haz clic en "Añadir Feed" en la barra de navegación superior.
2. **Introduce la URL**: Pega la URL de un feed ATOM o RSS (ejemplos recomendados abajo).
3. **Navega por las noticias**: Utiliza la paginación en la parte inferior para ver más noticias.
4. **Buscar noticias**: Escribe en el campo de búsqueda para filtrar las noticias mostradas.
5. **Guardar favoritos**: Haz clic en el botón "Favorito" para guardar una noticia y poder acceder a ella después.
6. **Ver favoritos**: Haz clic en "Favoritos" en la barra de navegación para ver solo tus noticias guardadas.

## Feeds recomendados

Puedes probar la aplicación con estos feeds:

- **Vandal**: `https://vandal.elespanol.com/xml.cgi` o `https://vandal.elespanol.com/rss/`
- **BBC News**: `https://feeds.bbci.co.uk/news/rss.xml`
- **New York Times**: `https://rss.nytimes.com/services/xml/rss/nyt/World.xml`
- **W3C (ATOM)**: `https://www.w3.org/blog/news/feed/atom`

## Tecnologías utilizadas

- **HTML5**: Estructura semántica moderna
- **CSS3**: Variables CSS para temas consistentes
- **JavaScript**: Vanilla JS sin dependencias adicionales
- **Bootstrap 5**: Framework CSS para componentes responsivos
- **Bootstrap Icons**: Iconografía moderna y limpia

## Estructura del proyecto

```
lector-rss/
├── index.html          # Página principal
├── css/
│   └── style.css       # Estilos personalizados
├── script/
│   └── app.js          # Lógica de la aplicación
└── image/
    └── placeholder.png # Imagen por defecto
```

## Instalación y ejecución local

1. Clona o descarga este repositorio
2. No se requiere instalación o configuración adicional
3. Abre el archivo `index.html` en un navegador moderno
4. (Opcional) Para mejor funcionamiento, puedes usar un servidor local:
   - Con Python: `python -m http.server`
   - Con Node.js: `npx serve`

## Solución de problemas

- **Error de CORS**: Si un feed no carga, la aplicación intentará usar un proxy. Si sigue fallando, prueba con otro feed.
- **Imágenes no visibles**: Algunas fuentes RSS/ATOM no incluyen imágenes. La aplicación mostrará una imagen por defecto.
- **Feed no reconocido**: Asegúrate de que la URL proporcionada sea un feed ATOM o RSS válido.

## Créditos

- Desarrollado como proyecto educativo
- Usa [Bootstrap](https://getbootstrap.com/) para la interfaz
- Proxy CORS proporcionado por [AllOrigins](https://allorigins.win/)

## Licencia

Este proyecto está bajo licencia MIT. Eres libre de usar, modificar y distribuir este código como desees.
