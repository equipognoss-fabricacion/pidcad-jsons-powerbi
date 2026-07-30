**Carpeta INE Experimental Medición teléfonos móviles**

Datos del INE de la "Estadística experimental. Medición del turismo a partir de teléfonos móviles", recuperada desde https://www.ine.es/dynt3/inebase/es/index.htm?padre=8578\&capsel=8579. Estos datos se pueden filtrar por los dos municipios que componen la comarca "Campiña de Jerez" (Jerez de la Frontera y San José del Valle) y cargar sólo los datos que interesan al caso



**2076.xlsx**

Ocupación hotelera (Establecimientos, plazas estimadas, grados de ocupación y personal empleado por puntos turísticos) por meses, para los municipios afectados (usar la fila de Jerez)



**Alojamientos\_zona\_jerez.xlsx**

Obtenido manualmente de https://www.cadizturismointeligente.es/, filtrando por la comarca "Campiña de Jerez".



**marco\_de\_jerez v2.xlsx**

Datos obtenidos del procesamiento del informe de ACEVIN. 

https://wineroutesofspain.com/wp-content/uploads/2025/10/informe-visitas-a-bodegas-y-museos-rutas-del-vino-de-espana-2024.pdf 

Contiene datos de:

* Total de servicios y entidades
* Visitantes a bodegas y museos
* Visitantes internacionales y nacionales
* Precio medio de visita a Bodegas y Museos
* Gasto medio en tienda de Bodegas y Museos
* Ingresos totales





**RTA\_Jerez.json**

Censo de alojamientos por municipio, desde el API de OPEN RTA (Registro de Turismo de Andalucía)

```
curl -X 'GET' \
  'https://datos.juntadeandalucia.es/api/v0/openrta/search?id=-\&object\_type=-\&category=-\&group=-\&modality=-\&province=-\&municipality=JEREZ%20DE%20LA%20FRONTERA\&order\_by=id\&mode=DESC\&format=json\&size=0\&object\_type\_id=0' \
  -H 'accept: application/json'
```


**Visitantes\_enoturismo\_Jerez.xlsx** 

Obtenido manualmente de https://siit.jerez.es/VisitantesPublicStats, filtrando por “BODEGAS”.



**Viviendas\_Turisticas\_Zona\_Jerez.xlsx**

Obtenido manualmente de https://www.cadizturismointeligente.es/, filtrando por la comarca "Campiña de Jerez".









