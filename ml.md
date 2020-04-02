# Lenguaje para Modelado de clases(ML)

> Referencia para el uso del lenguaje de modelado ML.

* Para declarar un **Modelo o Clase**:

```[ml]
[CLASSNAME]:c{[UI_NAME]|[COLLECTION_CLASSNAME]}[SOURCENAME]
```

```[ml]
Persona:c{Persona|Personas}[tblPesonas]
Persona:*#{Persona Id}[intPersona]
Nombre:ts{Nombre}[strNombre]
Apellido:s
Sexo:Sexo
Nacionalidad:auto
Telefonos:*Telefono?Persona:i
```

## Tipos de Propiedades

* Para definir una **Propiedad Simple**:
> Es decir que incluye un tipo de dato básico(string,integer,float,etc.)

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

* Para definir una **Propiedad Llave Objeto(Modelo)**:

```[ml]
[PROPERTY_NAME]:**[CLASSNAME]
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

* Para incluir un **Texto para la UI**:

```[ml]
[PROPERTY_NAME]:[PROPERTY_TYPE]{[NAME_FOR_UI] }
```

## Tipos de datos

Tipo de Dato ML | Tipo de Dato |Utilidad
------------------|--------------|-----------
s|String|para al almacenar texto corto
i|Integer|para al almacenar numeros enteros
t|String|para al almacenar texto largo
ts|String|para al almacenar descriptivo
x|Decimal|para al almacenar numeros decimales
l|Integer|para al almacenar numeros enteros
b|BLOB|para al almacenar contenido binario,archivo,etc.
0|boolean|para al almacenar valor cierto o falso
f|Float|para al almacenar numeros de punto flotante
d|DateTime|para al almacenar Fechas
ss|String|para al almacenar listado de string
y|Tinyint|para al almacenar numeros pequeños
256|String|para almacenar un string de longitud 256
