# models
Referencia para el uso del lenguaje de modelado ML.

## Lenguaje para Modelado
* Para declarar una **Clase**:
```[ml]
[CLASSNAME]:c
```
```[ml]
Persona:c
Persona:*#
Nombre:ts
```
## Tipos de Propiedades

* Para definir una **Propiedad Llave** numérica:
```[ml]
[PROPERTY_NAME]:i*
```
* Para definir una **Propiedad Llave** auto numérica:
```[ml]
[PROPERTY_NAME]:*#
```

* Para definir una **Propiedad Descriptiva**:
```[ml]
[PROPERTY_NAME]:ts
```



* Para definir una **Propiedad Objeto(Modelo)**:
```[ml]
[PROPERTY_NAME]:[CLASSNAME|auto]
```

* Para definir una **Propiedad Lista**:
```[ml]
[PROPERTY_NAME]:*[CLASSNAME]?[PROPERTY_FK]:[TYPE]
```
## Tipos de datos

Tipo de Dato Base | Descripcion
------------------|------------
s| Texto Corto
t| Texto Largo
i| Número Entero
l| Número Largo
ts| Texto Descriptivo
d| Fecha
b| Blob, Image
f| Numero Flotante
0| Booleano
x| Decimal