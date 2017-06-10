# models
Referencia para el uso del lenguaje de modelado ML.

## Lenguaje para Modelado
* Para declarar una **Clase**:
```[ml]
[CLASSNAME]:c{[UI_NAME]|[COLLECTION_CLASSNAME]}
```
```[ml]
Persona:c
Persona:*#
Nombre:ts
Apellido:s
Sexo:Sexo
```
## Tipos de Propiedades

* Para definir una **Propiedad Simple**:
```[ml]
[PROPERTY_NAME]:[PROPERTY_TYPE]
```

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
* Para definir una **Propiedad Auxiliar**:
```[ml]
[PROPERTY_NAME]:[PROPERTY_TYPE]!
```

## Tipos de datos

Tipo de Dato ML | Tipo de Dato |Utilidad
------------------|--------------|-----------
s|	String	|para al almacenar texto corto
i|	Integer	|para al almacenar numeros enteros
t|	String	|para al almacenar texto largo
ts|	String	|para al almacenar descriptivo
x|	Decimal	|para al almacenar numeros decimales
l|	Integer	|para al almacenar numeros enteros
b|	BLOB	|para al almacenar contenido binario,archivo,etc.
0|	boolean	|para al almacenar valor cierto o falso
f|	Float	|para al almacenar numeros de punto flotante
d|	DateTime	|para al almacenar Fechas
ss|	String	|para al almacenar listado de string
y|	Tinyint	|para al almacenar numeros pequeños