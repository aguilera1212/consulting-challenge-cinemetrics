# Consulting Challenge — CineMetrics

## Descripcion del proyecto y obejtivo del cliente

CineMetrics es una empresa que quiere saber si invertir en la película "A Minecraft Movie" (2025) fue una buena decisión. Este proyecto analiza con datos cuánto dinero ganó, cómo la calificó el público y cuánto interés generó en internet.

Para entenderlo mejor, la compara con otras películas basadas en videojuegos. Al final, el análisis ayuda a decidir si conviene invertir en futuras adaptaciones de videojuegos con presupuestos altos.

Los datos salen de TMDB y OMDb (recaudación, presupuesto y calificaciones) y de Google Trends (interés del público a lo largo del tiempo).

## Fuentes previstas

- **TMDB API:** presupuesto, recaudación, fecha de estreno, popularidad y títulos comparables.
- **OMDb API:** calificaciones agregadas de IMDb, Rotten Tomatoes y Metacritic cuando estén disponibles.
- **Google Trends / pytrends:** evolución del interés de búsqueda. Se documentará cualquier limitación de acceso o rate limit.

## Metodologia utlizada

Extracción: obtuvimos los datos de las películas desde las APIs de TMDB y OMDb y de Google Trends.
Limpieza: eliminamos duplicados, completamos o descartamos valores vacíos y corregimos los tipos de datos.
Análisis exploratorio: revisamos estadísticas, distribuciones y relaciones entre variables, y buscamos valores atípicos.
Visualización: armamos gráficos para comparar “A Minecraft Movie” con otras adaptaciones de videojuegos.
Hallazgos y recomendaciones: interpretamos los resultados y los traducimos en recomendaciones para el cliente.

## Principales hallazgos

Éxito comercial: "A Minecraft Movie" costó 150 millones de dólares y recaudó cerca de 960 millones, más de 6 veces su presupuesto. Superó ampliamente a otras adaptaciones de 2025, como Five Nights at Freddy's 2 (238 millones) y Until Dawn (54 millones).

Opinión dividida: La crítica la calificó con 45/100, mientras que el público le dio entre 56 y 62. A los críticos les pareció una historia simple que prioriza el espectáculo, pero la audiencia la disfrutó por el elenco, el humor y la nostalgia de ver su videojuego favorito en pantalla.

Impacto viral: El interés de búsqueda tuvo su pico el 5 de abril, un día después del estreno, y volvió a subir los días 10 y 11 por el meme del Chicken Jockey. Un fenómeno viral puede mantener vivo el interés por una película.

## Recomendaciones

1. Invertir en más adaptaciones de videojuegos, priorizando franquicias con una comunidad grande de fans, ya que "A Minecraft Movie" multiplicó por 6 su inversión.
2. No depender de la crítica para proyectar resultados: la película recaudó mucho con una calificación baja de los críticos, porque el público fue lo que la impulsó.
3. Aprovechar los momentos virales en la promoción: con campañas en redes que acompañen memes o tendencias después del estreno, para sostener el interés.

## Estructura

```text
data/raw/         # Respuestas originales descargadas desde las fuentes
data/processed/   # Datos limpios y listos para el análisis
notebooks/        # Extracción, limpieza y análisis exploratorio
images/           # Gráficos exportados para la presentación
presentation/     # Presentación ejecutiva final
```

## Estado actual

Proyecto finalizado a espera de revision del cliente

## Reproducción

1. Crear un entorno virtual de Python.
2. Instalar las dependencias con `pip install -r requirements.txt`.
3. Copiar `.env.example` como `.env` y completar las claves de API propias.
4. Ejecutar los notebooks en el orden numérico indicado.

## Limitaciones iniciales

- El presupuesto y la recaudación publicados pueden ser estimaciones o no contemplar costos de marketing.
- La popularidad o el interés de búsqueda no prueban por sí solos una relación causal con la recaudación.
- La recepción de audiencia puede estar condicionada por edad, marketing y composición de la muestra.
