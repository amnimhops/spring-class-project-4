# spring-class-project-4

_Restaurant API_

## 1. Introducción

En este proyecto se evaluará la capacidad de crear un proyecto _Spring_ en todas sus capas. Para ello, se propone la elaboración de la API de un restaurante, cuyo propósito es proveer las herramientas para alimentar a la aplicación con información a partir de la cual elaborar los platos.

Esta API se encarga de gestionar el menú de un restaurante, lo que incluye platos, 
ingredientes, alérgenos y unidades de medida. En general, cada plato tiene una serie de ingredientes
en una cantidad determinada, y su coste de compra y venta depende del precio de estos y de la cantidad asignada. Por su parte, cada ingrediente tiene una lista de alérgenos para que los clientes lo tengan en cuenta a la hora de elegir la comida. Además, cada ingrediente se expresa en una unidad de medida diferente. Por ejemplo, mientras que el "aceite" se expresa en mililitros, el "pollo" se expresa en gramos.

La documentación completa de la API puede encontrarse en la carpeta `docs/` en formato _markdown_, abriendo el archivo [**README.md**](docs/README.md)
## 2. Objetivo

La implementación de la API consta de 5 fases:
1. Análisis de la documentación facilitada
2. Creación de las clases de los controladores y los _beans_ de entrada y salida
3. Creación de las interfaces e implementaciones de los servicios necesarios
4. Propuesta y diseño de los modelos de datos subyacentes
5. Creación de los repositorios JPA necesarios para gestionar el modelo

## 3. Detalles de la API

### 3.1 Unidades de medida

Este tipo de dato sirve como soporte para indicar cuantas unidades de cada ingrediente consta cada plato. Según la especificación habrá que implementar las siguientes operaciones:

- Creación
- Actualización
- Consulta individual
- Listado filtrado y ordenado
- Baja

### 3.2 Alérgenos

Un ingrediente puede contener varios tipos de alérgenos, y para poder asignar un alérgeno a un ingrediente este debe estar primero registrado en el sistema. Las operaciones del endpoint `/restaurant/allergens` son:

- Creación
- Actualización
- Consulta individual
- Listado filtrado y ordenado
- Baja

Se deben cumplir las siguientes reglas:
- Si se intenta dar de baja un alérgeno vinculado a un ingrediente, se lanzará un error del tipo adecuado

### 3.3 Ingredientes

Un ingrediente es cada uno de los diferentes componentes que integran un plato. Un plato puede tener muchos ingredientes, así como un ingrediente puede estar presente en muchos platos. La relación entre un plato y un ingrediente tiene un atributo adicional que es la **cantidad**. Por ejemplo, cuando agregamos a un plato de "Pizza 4 quesos" el ingrediente "queso emmental", lo hacemos usando 100g de este ingrediente. El endpoint `/restaurant/ingredients` tendrá las siguientes operaciones:

- Creación
- Actualización
- Consulta individual
- Listado filtrado y ordenado
- Baja

Se deben cumplir las siguientes reglas:
- Si al dar de alta un ingrediente no existe la unidad de medida asociada, se lanzará un error del tipo adecuado
- Si al dar de alta un ingrediente no existe el alérgeno proporcionado, se lanzará un error del tipo adecuado
- Si se intenta dar de baja un ingrediente vinculado a un plato, se lanzará un error del tipo adecuado
- Al consultar la información de un ingrediente, se obtendrá también información sobre qué platos lo incorporan.

### 3.4 Platos

Un plato es una preparación que incorpora una determinada cantidad de ingredientes de cada tipo. Cada plato tiene un valor de compraventa que depende de las proporciones usadas de cada uno. El endpoint `/restaurant/dishes` tendrá las siguientes operaciones:

- Creación
- Actualización
- Consulta individual
- Listado filtrado y **paginado**
- Baja

Se deben cumplir las siguientes reglas:

- Al dar de baja un plato se conservarán las definiciones de los ingredientes, de manera que puedan utilizarse en otras preparaciones.
- Si al dar de alta un plato no existe el ingrediente indicado, se lanzará un error del tipo adecuado
- Si al dar de alta un plato se especifica un valor negativo o cero para un ingrediente determinado, se lanzará un error del tipo adecuado.

## 4. Organización del código y decisiones de diseño

Tanto la organización del código como las decisiones de diseño son completamente libres. Todo el modelo de datos subyacente solo debe servir a tres propositos: almacenar los datos a largo plazo, mantener la coherencia de los datos de acuerdo a lo indicado en la documentación de la API y satisfacer las reglas indicadas en este documento.