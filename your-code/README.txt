Este proyecto tiene 2 partes:
1. Web Scraping:
    Para esta sección descargué los libros escritos por Stephen King, directamente de la página del autor.
    La información contiene:
        Nombre del libro
        Fecha de publicación
        Tipo de libro (Novela, historia corta, etc.)
        Link al detalle del libro
    Esta información fue agregada a un DataFrame y exportada como archivo .csv
    Tras la verificación de los robots.txt, identifiqué que la página no permite la descarga de imágenes
2.  API
    Para esta sección ingresé a la página de Banxico para descargar las series de tiempo de:
        Tipo de cambio FIX
        Tasa de interés objetivo
        Nivel de UDIS
    Para descargar la información desde esta API, Banxico solicita la generación de un token
    El token fue removido del código, está disponible bajo solicitud
    La información fue extraida como series de tiempo y luego procesada en DataFrames independientes
    Posteriormente, fue unida bajo el mismo DataFrame.
    Una de las limitantes es que las fechas de inicio de las series de tiempo no coinciden
    Lo anterior limita el tamaño de la serie de datos finales