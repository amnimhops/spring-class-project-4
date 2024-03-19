# AllergensApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addAllergen**](AllergensApi.md#addAllergen) | **POST** /restaurant/allergens | Agrega un nuevo alérgeno |
| [**getAllergen**](AllergensApi.md#getAllergen) | **GET** /restaurant/allergens/{id} | Devuelve la información de un alérgeno |
| [**listAllergens**](AllergensApi.md#listAllergens) | **GET** /restaurant/allergens | Devuelve un listado de alérgenos, ordenado alfabéticamente y filtrado |
| [**updateAllergen**](AllergensApi.md#updateAllergen) | **PUT** /restaurant/allergens/{id} | Actualiza los datos de un alérgeno |


<a name="addAllergen"></a>
# **addAllergen**
> String addAllergen(CreateAllergen)

Agrega un nuevo alérgeno

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **CreateAllergen** | [**CreateAllergen**](../Models/CreateAllergen.md)| Información para dar de alta el nuevo alérgeno | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

<a name="getAllergen"></a>
# **getAllergen**
> AllergenDetails getAllergen(id)

Devuelve la información de un alérgeno

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del alérgeno | [default to null] |

### Return type

[**AllergenDetails**](../Models/AllergenDetails.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="listAllergens"></a>
# **listAllergens**
> List listAllergens(filter)

Devuelve un listado de alérgenos, ordenado alfabéticamente y filtrado

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **filter** | **String**| Permite filtrar los resultados para aquellos elementos cuyos atributos coincidan parcialmente con el texto indicado. | [optional] [default to null] |

### Return type

[**List**](../Models/Allergen.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="updateAllergen"></a>
# **updateAllergen**
> String updateAllergen(id, UpdateAllergen)

Actualiza los datos de un alérgeno

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del alérgeno | [default to null] |
| **UpdateAllergen** | [**UpdateAllergen**](../Models/UpdateAllergen.md)| Información para modificar el alérgeno | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

