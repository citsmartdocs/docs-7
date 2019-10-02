Title: Gestionar indización de contenido

# Gestionar Indización de Contenido

CITSmart utiliza el Apache SOLR para indexar el contenido creado en la Gestión de Conocimiento y lo disponibiliza en el sistema de búsqueda del Portal de Conocimiento.

## Lo que hacer antes

Para que la Indización del conocimiento funcione correctamente, es necesario:

* [x] Instalar el componente Apache SOLR como se muestra en el [manual de instalación][1].

## Parametrizar el servicio de indización

1. Acceder al menú principal Parametrización > Parámetros CITSmart;
2. Configurar el parámetro 304 que indica la dirección URL del componente SOLR;

    ```sh
    http://localhost:8983/solr/collection_name
    ```

3. Configurar el parámetro 308 informando la cantidad de elementos a indexar a la vez;
4. Configurar el parámetro 332 que indica si la sincronización con el servidor de indización está activa;
5. Acceder al menú principal Sistema > Configuración> Gestión del conocimiento (Indexación) y haga clic en "Actualizar el servidor de índices".

## Gestionar contenido

1. Acceder al menú principal Sistema > Configuración > Gestión del conocimiento (Indexación);
2. Para indizar los conocimientos disponibles, haga clic en "Indexar la base de conocimiento", o para eliminar los conocimientos ya
indexados, haga clic en "Eliminar la indexación de la base de conocimiento".


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>06/25/2019

[1]:/es-es/citsmart-7/get-started/installation-and-upgrade/download-software.html#servidor-de-indexacion-apache-solr
