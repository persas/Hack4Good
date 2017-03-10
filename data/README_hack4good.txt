DESCRIPCIÓN DE LOS DATASETS PARA LUCA-HACKFORGOOD 2017

Rango de fechas de los 3 datasets: 1 de febrero a 30 de abril de 2015


Dataset para mapear los códigos de departamento y municipio con sus nombres y geometrías:
https://github.com/santiblanko/colombia.geojson
Se ha utilizado el campo 'WCOLGEN02_' como código de municipio ('cod_mpio', 'cod_mpio_origin' y 'cod_mpio_destination' en los siguientes datasets)
Se ha utilizado el campo 'DPTO' como código de departamento ('cod_dpto' en los siguientes datasets)


hack4good_dwells.csv:
* date_dt: fecha en la que tuvieron lugar las estancias.
* cod_dpto: código de departamento de Colombia (similar a Comunidad Autónoma en España).
* cod_mpio: código de municipio de Colombia (similar a municipio en España)
* dwells: número de estancias detectadas (se considera estancia a permanencia en un lugar aproximadamente a partir de 2h)
* people: número de personas distintas para las que se detectaron las estancias

hack4good_journeys.csv:
* date_dt: fecha en la que tuvieron lugar los desplazamientos de ese registro.
* cod_mpio_origin: código de municipio de Colombia (similar a municipio en España) desde el que se iniciaron los desplazamientos contabilizados en ese registro (hay un registro por cada combinación fecha-origen-destino).
* cod_mpio_destination: código de municipio de Colombia (similar a municipio en España) en el que finalizaron los desplazamientos contabilizados en ese registro (hay un registro por cada combinación fecha-origen-destino).
* journeys: número de desplazamientos detectados.
* people: número de personas distintas para las que se detectaron los desplazamientos.

hack4good_antenas.csv:
Todos los campos de hack4good_antenas.csv excepto date_dt, cod_dpto y cod_mpio pueden contener nulos (NaNs).
* date_dt: fecha de observación del tráfico de antenas en el municipio.
* cod_dpto: código de departamento de Colombia (similar a Comunidad Autónoma en España).
* cod_mpio: código de municipio de Colombia (similar a municipio en España).
* 3g_traf_dl: datos 3G de descarga (MB).
* 3g_traf_ul: datos 3G de subida (MB).
* 3g_completadas: número de llamadas completadas vía red 3G.
* 3g_no_completadas: número de llamadas no completadas vía red 3G.
* 2g_traf_dl: datos 2G de descarga (MB).
* 2g_traf_ul: datos 2G de subida (MB).
* 2g_completadas: número de llamadas completadas vía red 2G.
* 2g_no_completadas: número de llamadas no completadas vía red 2G.
