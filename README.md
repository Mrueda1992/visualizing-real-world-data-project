<h2> VISUALIZATING REAL WORLD DATA PROJECT </h2>

El propósito de este proyecto consistía en seleccionar la ubicación idónea para una futura empresa del sector de los videojuegos. La decisión ha sido tomada en base a unas consideraciones previas a la realización del proyecto, sirviendo como criterios iniciales para realizar una limpieza y un análisis de los datos del primer dataset, así como su posterior enriquecimiento mediante datos obtenidos de la API de Google Places.

Los requisitos principales para situar nuestra empresa han sido: 

1. El valor, entendido como la suma de las cotizaciones, de las empresas que operaban en una misma zona geográfica.
2. La existencia de empresas importantes pertenecientes al sector de los videojuegos, categorizadas en el dataset como "games_video".
3. El hecho de que en esta zona haya espacios de conveniencia, tales como guarderías, cafés o pubs, cerca de la oficina.

En el repositorio podemos encontrar el proceso de limpieza y análisis de datos que han llevado a la selección de la ubicación de la empresa, que será en Santa Mónica (Los Ángeles, USA). En primer lugar, en el archivo llamado "cleaning" hemos hecho una query en MongoDB de la cual hemos extraido una primera muestra de empresas. Después, hemos procedido a la creación de un dataset que contuviese de forma legible las empresas cuya ubicación nos interesa. Para volver a filtrar el dataset mediante una segunda query, creamos el archivo "second_filter", que solo contiene la nueva query mencionada. Con esto, llegamos al documento final, "geoquery", que finaliza el análisis, creamos un mapa con Folium, una librería de Python especializada en visualización para análisis de datos, y, en base a los criterios mencionados para seleccionar la ubicación de la empresa, buscamos en la zona elegida los lugares de conveniencia mediante llamadas a la API de Google.

