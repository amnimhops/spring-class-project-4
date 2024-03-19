# IngredientsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addIngredient**](IngredientsApi.md#addIngredient) | **POST** /restaurant/ingredients | Agrega un nuevo ingrediente |
| [**deleteIngredient**](IngredientsApi.md#deleteIngredient) | **DELETE** /restaurant/ingredient/{id} | Elimina un ingrediente |
| [**getIngredient**](IngredientsApi.md#getIngredient) | **GET** /restaurant/ingredient/{id} | Devuelve la información de un ingrediente |
| [**listIngredients**](IngredientsApi.md#listIngredients) | **GET** /restaurant/ingredients | Devuelve un listado de los ingredientes disponibles, ordenados alfabéticamente y filtrados |
| [**updateIngredient**](IngredientsApi.md#updateIngredient) | **PUT** /restaurant/ingredient/{id} | Actualiza una unidad de medida |


<a name="addIngredient"></a>
# **addIngredient**
> String addIngredient(CreateIngredient)

Agrega un nuevo ingrediente

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **CreateIngredient** | [**CreateIngredient**](../Models/CreateIngredient.md)| Información para dar de alta el nuevo ingrediente | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

<a name="deleteIngredient"></a>
# **deleteIngredient**
> String deleteIngredient(id)

Elimina un ingrediente

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del ingrediente | [default to null] |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain

<a name="getIngredient"></a>
# **getIngredient**
> IngredientDetails getIngredient(id)

Devuelve la información de un ingrediente

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del ingrediente | [default to null] |

### Return type

[**IngredientDetails**](../Models/IngredientDetails.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="listIngredients"></a>
# **listIngredients**
> List listIngredients(filter)

Devuelve un listado de los ingredientes disponibles, ordenados alfabéticamente y filtrados

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **filter** | **String**| Permite filtrar los ingredientes cuyos atributos coincidan con el texto indicado | [optional] [default to null] |

### Return type

[**List**](../Models/Ingredient.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="updateIngredient"></a>
# **updateIngredient**
> String updateIngredient(id, UpdateIngredient)

Actualiza una unidad de medida

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del ingrediente | [default to null] |
| **UpdateIngredient** | [**UpdateIngredient**](../Models/UpdateIngredient.md)| Información para modificar el ingrediente | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

