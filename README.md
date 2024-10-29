<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Análisis Espacial de Casos de COVID-19 en Perú (2021) - Tarea 4</title>
</head>
<body>

<h1>Análisis Espacial de Casos de COVID-19 en Perú (2021) - Tarea 4</h1>

<h2>Introducción y Fuente de Datos</h2>
<p>
    Este análisis utiliza datos de casos positivos de COVID-19 proporcionados por el Ministerio de Salud de Perú (MINSA) a través de su plataforma de datos abiertos. 
    <a href="https://www.datosabiertos.gob.pe" target="_blank">Enlace a la base de datos</a>.
</p>

<h2>Metodología</h2>
<ul>
    <li><strong>Periodo de Análisis:</strong> Se analizaron los datos entre 2020 y 2024, con un enfoque específico en el año 2021.</li>
    <li><strong>Distribución Geográfica:</strong> Utilizamos datos geográficos a nivel de departamento y provincia, integrados mediante <em>geopandas</em> para visualizar los casos de COVID-19 en mapas de Perú.</li>
    <li><strong>Índice de Moran:</strong> Calculamos el índice de Moran global, que reveló una débil autocorrelación espacial positiva (I = 0.17), sugiriendo que áreas con altas (o bajas) tasas de casos tienden a estar cerca, pero esta relación no es fuerte.</li>
    <li><strong>Análisis LISA:</strong> Identificamos patrones locales de autocorrelación:
        <ul>
            <li><strong>HH (Alto-Alto):</strong> Clusters de alta incidencia, posibles focos de contagio.</li>
            <li><strong>LL (Bajo-Bajo):</strong> Zonas de baja incidencia.</li>
            <li><strong>HL (Alto-Bajo) y LH (Bajo-Alto):</strong> Outliers espaciales, áreas con tasas opuestas a sus vecinas.</li>
        </ul>
    </li>
    <li><strong>Visualización de Clusters:</strong> Los mapas LISA ayudan a ubicar espacialmente estas áreas críticas para la toma de decisiones de salud pública.</li>
    <li><strong>LISA Bivariado:</strong> Evaluamos la relación espacial entre los casos de COVID-19 en 2021 y 2022, identificando áreas donde la incidencia se mantuvo alta (HH) o baja (LL), lo cual es útil para estrategias de salud pública enfocadas en reducir la transmisión.</li>
</ul>

<h2>Resultados</h2>
<p>
    Todo el procedimiento se puede observar al detalle en el archivo HTML. . 
    <a href="[https://www.datosabiertos.gob.pe](https://michaelencalada.github.io/week10_spatial/Tarea4.html)" target="_blank">Tarea en Python</a>.
</p>


<h2>Visualización</h2>
<ul>
    <li><strong>Moran Scatterplot y Mapas de Clusters:</strong> Gráficos y mapas detallan la intensidad de los casos y la agrupación de valores altos y bajos a nivel provincial.</li>
    <li><strong>Gráficos:</strong> Índice de Moran</li> 
</ul>

</body>
</html>

