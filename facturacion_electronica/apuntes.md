# GroovyEvaluator not found

## Luego de modificar el jrxml con jasper irepors 5.6 se produce ese error

Pude resolver esto por:

quitar language="groovy"
(o) reemplazando language="groovy"con language="java"en mi JRXMLarchivo
No olvide guardar y compilar.
