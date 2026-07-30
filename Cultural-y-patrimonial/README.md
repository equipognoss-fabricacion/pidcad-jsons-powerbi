**Carpeta Dataestur**



**actividades\_ocio.xlsx**
Gastos en espectáculos culturales \[2024-2025-2026, por mes y categoría]
```
curl -X 'GET'   
'https://www.dataestur.es/API-SEGITTUR-v2/ACTIVIDADES\_OCIO\_DL?desde%20%28a%C3%B1o%29=2024\&desde%20%28mes%29=1\&hasta%20%28a%C3%B1o%29=2026\&hasta%20%28mes%29=6\&CCAA=Andaluc%C3%ADa\&Provincia=C%C3%A1diz'   
-H 'accept: application/vnd.ms-excel'
```
Las categorías de interés son: Cine; Conferencias; Cultura, teatro y danza; Música; Musicales
Se excluyen: Actividades infantiles; Cursos; Deportes y aventuras; Gastronomía
Datos disponibles:
ENTRADAS
VISITAS\_PAGINAS
GASTO\_TOTAL
PRECIO\_MEDIO\_ENTRADA
TRANSACCIONES



**atracciones\_recursos\_turisticos valoración.xlsx**

Valoración de recursos turísticos.

Obtención de la última valoración, del primer trimestre (se recomienda que la Diputación consiga las anteriores), para poder presentar la evolución por trimestres.

```
curl -X 'GET' \
  'https://www.dataestur.es/API-SEGITTUR-v2/ATRACCIONES\_RECURSOS\_TURISTICOS\_DL?Provincia=C%C3%A1diz' \
  -H 'accept: application/octet-stream'
```


**Carpeta Junta de Andalucía**



**Museo de Cádiz 2024.xlsx**

Visitas al Museo de Cádiz \[2024, por tipo de actividad] (fuente Junta de Andalucía)

Personas usuarias por mes, de 2024, 2025 y 2026

https://www.juntadeandalucia.es/sites/default/files/2025-11/museos24_0.xlsx

En la Hoja “3”

https://www.juntadeandalucia.es/sites/default/files/2026-05/museos25_12_V2.xlsx

https://www.juntadeandalucia.es/sites/default/files/2026-07/museos26_05.xlsx



Desglose de visitas anuales de 2024:

individual y grupos, hombres y mujeres

Tipo de actividad: visitas guiadas, talleres, etc.

https://www.juntadeandalucia.es/sites/default/files/2025-11/museos24_0.xlsx

En la Hoja “21”





**Actividades\_Cadiz\_AgendaCultural.xlsx**

Generado como una carga inicial desde un proceso de crawler. Debería formar parte de la fuente de eventos con la que se actualice el grafo del CMS Semántico



**BienesInmuebles.json y BienesInmuebles2.json**

Consulta de Bienes inmuebles:

https://www.juntadeandalucia.es/datosabiertos/portal/dataset/patrimonio-inmueble-de-andalucia

Caracterización (no exhaustiva): Arqueológica, Arquitectónica, Etnológica, Sin Caracterización

Atributos de alineación con la ontología:

"den\_tipologia"  p.e. "Palacios"; “Mezquitas” y “Torres”

"tipologia\_smv" p.e. "Palacios"



Llamadas al API para obtener los datos:

https://guiadigital.iaph.es/store/apis/info?name=open-data-iaph\&version=1.0\&provider=guiadigital

```
curl -k -X GET "https://guiadigital.iaph.es/api/1.0/bien/inmueble/2097" -H "accept: application/json" -H "Authorization: Bearer ebe7d5fd-e77c-3581-8242-6eb6a5dbdbef"
```



**consumo\_cultural\_cadiz v3.xlsx**

Datos preparados manualmente, con visitantes al Teatro Romano de Cádiz (hoja "Consumo cultural")



**dataset-orbe\_museos.json**

Consulta de Museos de Andalucía, filtrable por provincia al cargar en PowerBI

https://www.juntadeandalucia.es/datosabiertos/portal/dataset/museos-de-andalucia

https://datos.juntadeandalucia.es/api/v0/museums/all?format=json



**ECTA\_Cadiz\_2022-2024\_Gastos\_por\_Actividad.xlsx**

Gastos por tipo de actividad \[2022-2024, por meses], de la fuente ECTA Encuesta de Coyuntura Turística de Andalucía (ECTA)

del Instituto de Estadística y Cartografía de Andalucía

https://ws089.juntadeandalucia.es/indea-gestion/restServices/v.2.0/datosSerie?codIndicador=ECTAn3497\&codTerritorio=11\&numPeriodos=24\&iniPeriodo=\&finPeriodo=\&formato=

El documento incluye datos extrapolados que se suponen disponibles en el Banco de Datos Estadísticos de Andalucía (BADEA)



**PatrimonioCulturalInmaterial.json**

Consulta de Patrimonio cultural inmaterial:

https://www.juntadeandalucia.es/datosabiertos/portal/dataset/patrimonio-inmaterial-de-andalucia 

Atributos de alineación con la ontología:

"ambito"  p.e. "Rituales festivos”, “Oficios y saberes”, “Alimentación y sistemas culinarios”

“tipologías” p.e. “Viticultura”, “Repostería”

Llamadas al API para obtener los datos:

https://guiadigital.iaph.es/store/apis/info?name=open-data-iaph\&version=1.0\&provider=guiadigital 

```
curl -k -X GET "https://guiadigital.iaph.es/api/1.0/bien/inmaterial/218472" -H "accept: application/json" -H "Authorization: Bearer ebe7d5fd-e77c-3581-8242-6eb6a5dbdbef"
```


**rutas-culturales.json**

Consulta de Rutas

https://www.juntadeandalucia.es/datosabiertos/portal/dataset/rutas-culturales



**Visitantes\_Teatro\_Romano\_Baelo\_Claudia.xlsx**

Simulación con datos macro de visitantes del Teatro Romano y de Baelo Claudia \[2022-2025, por meses] 

El documento incluye datos extrapolados



