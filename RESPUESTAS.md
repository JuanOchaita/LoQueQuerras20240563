# Juan Ochaita

# Respuestas

- `Jenkinsfile`, ejecución de regresión: se eliminó `|| true`, porque ocultaba los fallos de Bruno y permitía que el pipeline continuara como si hubiera pasado.
- `Jenkinsfile`, publicación JUnit: se cambió `bruno/smoke/results.xml` por `bruno/regresion/results.xml`, porque se estaba publicando el reporte de una suite distinta.
- `Jenkinsfile`, publicación JUnit: se eliminó `allowEmptyResults: true`, porque permitía que Jenkins quedara verde aunque no existiera ningún reporte.

## Builds de P3

Esta entrega contiene la versión funcional completa en un solo commit. Los números y SHA de los tres builds secuenciales de P3 deben agregarse después de ejecutarlos en Jenkins, respetando el orden indicado en el README.

## Aserción fallida del build rojo

La aserción que debe fallar antes de corregir `api.py` es `res.body.monto: eq 60`.
