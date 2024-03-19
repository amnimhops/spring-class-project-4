# MeasuresApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addMeasure**](MeasuresApi.md#addMeasure) | **POST** /restaurant/measures | Agrega una nueva unidad de medida |
| [**deleteAllergen**](MeasuresApi.md#deleteAllergen) | **DELETE** /restaurant/allergens/{id} | Elimina un alérgeno |
| [**deleteMeasure**](MeasuresApi.md#deleteMeasure) | **DELETE** /restaurant/measures/{id} | Elimina una unidad de medida |
| [**getMeasure**](MeasuresApi.md#getMeasure) | **GET** /restaurant/measures/{id} | Devuelve la información de una unidad de medida |
| [**listMeasures**](MeasuresApi.md#listMeasures) | **GET** /restaurant/measures | Devuelve un listado de unidades de medida disponibles, ordenadas alfabéticamente |
| [**updateMeasure**](MeasuresApi.md#updateMeasure) | **PUT** /restaurant/measures/{id} | Actualiza una unidad de medida |


<a name="addMeasure"></a>
# **addMeasure**
> String addMeasure(CreateMeasure)

Agrega una nueva unidad de medida

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **CreateMeasure** | [**CreateMeasure**](../Models/CreateMeasure.md)| Información para dar de alta la nueva unidad de medida | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

<a name="deleteAllergen"></a>
# **deleteAllergen**
> String deleteAllergen(id)

Elimina un alérgeno

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador del alérgeno | [default to null] |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain

<a name="deleteMeasure"></a>
# **deleteMeasure**
> String deleteMeasure(id)

Elimina una unidad de medida

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador de la unidad | [default to null] |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain

<a name="getMeasure"></a>
# **getMeasure**
> MeasureDetails getMeasure(id)

Devuelve la información de una unidad de medida

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador de la unidad | [default to null] |

### Return type

[**MeasureDetails**](../Models/MeasureDetails.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="listMeasures"></a>
# **listMeasures**
> List listMeasures(filter)

Devuelve un listado de unidades de medida disponibles, ordenadas alfabéticamente

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **filter** | **String**| Permite filtrar las unidades de medida cuyo nombre coincida parcialmente con el texto indicado. | [optional] [default to null] |

### Return type

[**List**](../Models/Measure.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

<a name="updateMeasure"></a>
# **updateMeasure**
> String updateMeasure(id, UpdateMeasure)

Actualiza una unidad de medida

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Integer**| Identificador de la unidad | [default to null] |
| **UpdateMeasure** | [**UpdateMeasure**](../Models/UpdateMeasure.md)| Información para modificar la unidad de medida | |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/plain

