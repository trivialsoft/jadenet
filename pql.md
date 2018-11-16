## Definición del lenguaje PQL

Por: Antonio Ramírez Santander

* El lenguaje **PQL(Property Query Language)** es un lenguaje auxiliar 
de selección de propiedades de un modelo **ML**, el cual permite seleccionar ciertas propiedades de un modelo en una instruccion **fill** dentro de un **[T4U Template](T4UTemplate)**, a continuación se muestra las palabras claves que lo conforman.

|Instruccion PQL v1.0|PQL v2.0|Utilidad|
------------|--------|-------|
anyproperty           |.any|Selecciona cualquier propiedad
anypropertybasic      |.basic|Selecciona solo las propiedades basicas
anypropertyobject     |.object|Selecciona solo las propiedades objeto
anypropertydesc       |.desc|Selecciona solo las propiedades descriptivas   
anypropertykey        |.key|Selecciona solo las propiedades llave
anypropertylist       |.list|Selecciona solo las propiedades lista
anypropertyrule       |na|Selecciona solo las propiedades regla
anypropertyaux        |.aux|Selecciona solo las propiedades auxiliares basicas
anypropertyobjectaux  |.objectaux|Selecciona solo las propiedades auxiliares objeto
anyproperty:i         |.any:i|Selecciona solo las propiedades del tipo i
anyproperty:s         |.any:s|Selecciona solo las propiedades del tipo s
anyproperty:t         |.any:t|Selecciona solo las propiedades del tipo t
anyproperty:f         |.any:f|Selecciona solo las propiedades del tipo f
anyproperty:d         |.any:d|Selecciona solo las propiedades del tipo d
anyproperty:b         |.any:b|Selecciona solo las propiedades del tipo b
anyproperty:*#        |.any:#*|Selecciona solo las propiedades del tipo *#
anyproperty:#*        |.any:#*|Selecciona solo las propiedades del tipo #*
anyproperty:[OBJECTTYPE]  |.any:[OBJECTTYPE],.object:[OBJECTTYPE]|Donde OBJECTTYPE es un Modelo Selecciona las propiedad de ese Tipo
anypropertyobject.first|-|Selecciona solo la primera propiedad objeto
anyproperty.last |-| Selecciona la ultima propiedad del modelo
+[PROPERTY_GROUP]||Selecciona un grupo de propiedades
+![PROPERTY_GROUP]||Excluye un grupo de propiedades
![PROPERTY_NAME]||Excluye explicitamente una propiedad
![QUERYKEY_NAME]||Excluye explicitamente por querykey