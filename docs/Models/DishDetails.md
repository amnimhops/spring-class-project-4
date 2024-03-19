# DishDetails
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **id** | **Integer** | Identificador del plato | [optional] [default to null] |
| **name** | **String** | Nombre del plato | [optional] [default to null] |
| **description** | **String** | Descripción del plato para el menú | [optional] [default to null] |
| **dinners** | **Integer** | Indica el número de comensales indicados para este plato (orientativo) | [optional] [default to null] |
| **buyPrice** | **BigDecimal** | Indica el precio que le cuesta al restaurante comprar todos los materiales para elaborar este plato | [optional] [default to null] |
| **sellPrice** | **BigDecimal** | Indica el precio de venta al publico de este plato, basándose en el precio individual de cada ingrediente. | [optional] [default to null] |
| **ingredients** | [**List**](DishDetails_ingredients_inner.md) | Lista de ingredientes que incorpora este plato | [optional] [default to null] |
| **allergens** | [**List**](DishDetails_allergens_inner.md) | Lista de alérgenos de este plato | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

