# DishesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addDish**](DishesApi.md#addDish) | **POST** /restaurant/dishes | Agrega un nuevo plato al menu |
| [**deleteDish**](DishesApi.md#deleteDish) | **DELETE** /restaurant/dishes/{id} | Elimina un plato |
| [**getDish**](DishesApi.md#getDish) | **GET** /restaurant/dishes/{id} | Devuelve la información de un plato del menu |
| [**searchDish**](DishesApi.md#searchDish) | **GET** /restaurant/dishes | Busca los platos que cumplan el criterio de búsqueda |
| [**updateDish**](DishesApi.md#updateDish) | **PUT** /restaurant/dishes/{id} | Actualiza un plato |


<a name="addDish"></a>
# **addDish**
> String addDish(CreateDish)

Agrega un nuevo plato al menu

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **CreateDish** | [**CreateDish**](../Models/CreateDish.md)| Información del plato | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

<a name="deleteDish"></a>
# **deleteDish**
> String deleteDish(id)

Elimina un plato

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del plato | [default to null] |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain

<a name="getDish"></a>
# **getDish**
> DishDetails getDish(id)

Devuelve la información de un plato del menu

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del plato | [default to null] |

### Return type

[**DishDetails**](../Models/DishDetails.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="searchDish"></a>
# **searchDish**
> DishSearchResult searchDish(recordsPerpage, page, filter)

Busca los platos que cumplan el criterio de búsqueda

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **recordsPerpage** | **Integer**| Número de registros que deben devolverse en cada página de resultados. | [default to null] |
| **page** | **Integer**| Página de resultados que se desea devolver | [default to null] |
| **filter** | **String**| Criterio de búsqueda empleado para encontrar el plato. El filtro debe funcionar también con cualquier campo del plato, incluyendo ingredientes y alérgenos. | [optional] [default to null] |

### Return type

[**DishSearchResult**](../Models/DishSearchResult.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="updateDish"></a>
# **updateDish**
> String updateDish(id, UpdateDish)

Actualiza un plato

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del plato | [default to null] |
| **UpdateDish** | [**UpdateDish**](../Models/UpdateDish.md)| Información para modificar el plato | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

