
## Consulta ‘OAI-PMH’ Repositorio Nacional México 2023-2024


Aqui encuentra el código de R para las consultas OAI.
Se emplea el url que aún se encuentra disponible hasta 2026, aunque ésta puede ser descontinuada: https://oai-pmh.repositorionacionalcti.mx/resource/oai-pmh


Recomendación de artículo científico en el que se basa el código:

-   2016
-   Harvesting academic metadata through the OAI-PMH protocol to measure the impact of scientific
    (<https://www.pedrosantana.mx/preprints/rocc_2018_2019-harvesting_oai.pmh.pdf>)



## Instalar y cargar librias

Instalar

``` r
install.packages(c("OAIHarvester", "tidyverse", "rio", "readr", "writexl", "pacman", "openxlsx"))
```

Cargar paquetes con pacman

``` r
pacman::p_load(OAIHarvester, tidyverse, rio, readr, writexl, openxlsx)
```
Establecer la ruta para la escritura de las consultas
``` r
setwd("/home/alux/Documents/2026/LaReferencia/Mexico") #establecer la carpeta
```

## Variable URL OAI PMH del Repositorio Nacional México

Install from CRAN

``` r
baseurl <- "https://oai-pmh.repositorionacionalcti.mx/resource/oai-pmh"
```

## Variable "set_RN" con "List Set" de 108 instituciones, variable "baseurl" 

``` r
set_RN <- oaih_list_sets(baseurl,transform = TRUE)
```

## Unir dataframe resultado de la consulta 

``` r
rbind(set_RN, deparse.level = 0)
```

-   Dimensión Sets, 2823 filas y 3 columnas dataframe, febrero 2023
-   2848 15 de junio 2023
-   2890 11 de julio 2023
-   2892 1 de agosto 2023, # 2 de octubre 2023, noviembre no sirvió el SSL
-   2906 el 5 diciembre
-   2919 el 20 enero 2024
-   2920 el 26 de enero
-   2920 el 3 marzo 2024
-   2926 el 30 abril 2024
-   4 julio 2024  -durante los mes de julio, agosto, septiembre, octubre y hasta el 29 noviembre SSL vencido.
-   2926 el 9 diciembre 2024
-   2926 24 de marzo 2025


## Descargar el archivo RN_OAI_Harvester_Codigo_26_2_2024 para correr el código completo

-   Por favor descargue el archivo y antes de ejecutar seleccione la ruta donde se guardarán los archivos.

Gracias, Saludos.
