# Consulting Challenge — CineMetrics

## Objetivo

Evaluar si **A Minecraft Movie** (2025) fue una inversión exitosa para CineMetrics y si el patrón de crítica dividida, audiencia entusiasta y fenómeno viral justifica invertir en futuras adaptaciones de videojuegos de alto presupuesto.

## Preguntas de negocio

1. ¿El desempeño comercial de la película justifica considerarla una inversión exitosa?
2. ¿Cómo difieren la recepción de la crítica y la del público?
3. ¿El interés de búsqueda alrededor del estreno aporta evidencia de un fenómeno que pueda ser relevante para la decisión?

## Fuentes previstas

- **TMDB API:** presupuesto, recaudación, fecha de estreno, popularidad y títulos comparables.
- **OMDb API:** calificaciones agregadas de IMDb, Rotten Tomatoes y Metacritic cuando estén disponibles.
- **Google Trends / pytrends:** evolución del interés de búsqueda. Se documentará cualquier limitación de acceso o rate limit.

Las claves de API se guardarán únicamente en un archivo local `.env`, que no se sube al repositorio.

## Estructura

```text
data/raw/         # Respuestas originales descargadas desde las fuentes
data/processed/   # Datos limpios y listos para el análisis
notebooks/        # Extracción, limpieza y análisis exploratorio
images/           # Gráficos exportados para la presentación
presentation/     # Presentación ejecutiva final
```

## Estado actual

Proyecto inicializado. Próximo paso: obtener las credenciales de las APIs y construir el notebook de extracción.

## Reproducción

1. Crear un entorno virtual de Python.
2. Instalar las dependencias con `pip install -r requirements.txt`.
3. Copiar `.env.example` como `.env` y completar las claves de API propias.
4. Ejecutar los notebooks en el orden numérico indicado.

## Limitaciones iniciales

- El presupuesto y la recaudación publicados pueden ser estimaciones o no contemplar costos de marketing.
- La popularidad o el interés de búsqueda no prueban por sí solos una relación causal con la recaudación.
- La recepción de audiencia puede estar condicionada por edad, marketing y composición de la muestra.
