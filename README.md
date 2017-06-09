# models
Listado de Modelos ML para compartir

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

### Propiedad Lista

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