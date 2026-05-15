# Consulta del url OAI del Repositorio Nacional de Ciencia y Tecnología. México. Consejo Nacional de Ciencia y Tecnología. 
Uso de la Librería de R IOA-Harverster (CRAN) para la consulta de los items del repositorios de acceso abierto.

Aqui encuentra el código de R para las consultas OAI.
Se emplea el url que aún se encuentra disponible hasta 2026, aunque ésta puede ser descontinuada: https://oai-pmh.repositorionacionalcti.mx/resource/oai-pmh

También es recomendable consultar el texto de 2016 donde se haya la referencia del url antes mencionado. Consulte "Harvesting academic metadata through the OAI-PMH protocol to measure the impact of scientific", disponible en: https://www.pedrosantana.mx/preprints/rocc_2018_2019-harvesting_oai.pmh.pdf

### Repositorio Nacional OAI-PMH  ------------------------------------------------
# Se emplea paquete para consulta de url OAI PMH pública del Repositorio Nacional Conacyt
# Las consultas se hacen con base en los verbos y criterios del protocolo OAI.


# ****  Paquetes empleados ------------------------------------------------------
# Cargar paquete OAIHarvester: Harvest Metadata Using OAI-PMH Version 2.0

install.packages(c("OAIHarvester", "tidyverse", "rio", "readr", "writexl", "pacman", "openxlsx"))

Saludos.
