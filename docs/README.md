# Documentation for Ristorant API

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *http://localhost*

| Class | Method | HTTP request | Description |
|------------ | ------------- | ------------- | -------------|
| *AllergensApi* | [**addAllergen**](Apis/AllergensApi.md#addallergen) | **POST** /restaurant/allergens | Agrega un nuevo alérgeno |
*AllergensApi* | [**getAllergen**](Apis/AllergensApi.md#getallergen) | **GET** /restaurant/allergens/{id} | Devuelve la información de un alérgeno |
*AllergensApi* | [**listAllergens**](Apis/AllergensApi.md#listallergens) | **GET** /restaurant/allergens | Devuelve un listado de alérgenos, ordenado alfabéticamente y filtrado |
*AllergensApi* | [**updateAllergen**](Apis/AllergensApi.md#updateallergen) | **PUT** /restaurant/allergens/{id} | Actualiza los datos de un alérgeno |
| *DishesApi* | [**addDish**](Apis/DishesApi.md#adddish) | **POST** /restaurant/dishes | Agrega un nuevo plato al menu |
*DishesApi* | [**deleteDish**](Apis/DishesApi.md#deletedish) | **DELETE** /restaurant/dishes/{id} | Elimina un plato |
*DishesApi* | [**getDish**](Apis/DishesApi.md#getdish) | **GET** /restaurant/dishes/{id} | Devuelve la información de un plato del menu |
*DishesApi* | [**searchDish**](Apis/DishesApi.md#searchdish) | **GET** /restaurant/dishes | Busca los platos que cumplan el criterio de búsqueda |
*DishesApi* | [**updateDish**](Apis/DishesApi.md#updatedish) | **PUT** /restaurant/dishes/{id} | Actualiza un plato |
| *IngredientsApi* | [**addIngredient**](Apis/IngredientsApi.md#addingredient) | **POST** /restaurant/ingredients | Agrega un nuevo ingrediente |
*IngredientsApi* | [**deleteIngredient**](Apis/IngredientsApi.md#deleteingredient) | **DELETE** /restaurant/ingredient/{id} | Elimina un ingrediente |
*IngredientsApi* | [**getIngredient**](Apis/IngredientsApi.md#getingredient) | **GET** /restaurant/ingredient/{id} | Devuelve la información de un ingrediente |
*IngredientsApi* | [**listIngredients**](Apis/IngredientsApi.md#listingredients) | **GET** /restaurant/ingredients | Devuelve un listado de los ingredientes disponibles, ordenados alfabéticamente y filtrados |
*IngredientsApi* | [**updateIngredient**](Apis/IngredientsApi.md#updateingredient) | **PUT** /restaurant/ingredient/{id} | Actualiza una unidad de medida |
| *MeasuresApi* | [**addMeasure**](Apis/MeasuresApi.md#addmeasure) | **POST** /restaurant/measures | Agrega una nueva unidad de medida |
*MeasuresApi* | [**deleteAllergen**](Apis/MeasuresApi.md#deleteallergen) | **DELETE** /restaurant/allergens/{id} | Elimina un alérgeno |
*MeasuresApi* | [**deleteMeasure**](Apis/MeasuresApi.md#deletemeasure) | **DELETE** /restaurant/measures/{id} | Elimina una unidad de medida |
*MeasuresApi* | [**getMeasure**](Apis/MeasuresApi.md#getmeasure) | **GET** /restaurant/measures/{id} | Devuelve la información de una unidad de medida |
*MeasuresApi* | [**listMeasures**](Apis/MeasuresApi.md#listmeasures) | **GET** /restaurant/measures | Devuelve un listado de unidades de medida disponibles, ordenadas alfabéticamente |
*MeasuresApi* | [**updateMeasure**](Apis/MeasuresApi.md#updatemeasure) | **PUT** /restaurant/measures/{id} | Actualiza una unidad de medida |


<a name="documentation-for-models"></a>
## Documentation for Models

 - [Allergen](./Models/Allergen.md)
 - [AllergenDetails](./Models/AllergenDetails.md)
 - [AllergenDetails_allOf_presentIn](./Models/AllergenDetails_allOf_presentIn.md)
 - [AmountOfIngredient](./Models/AmountOfIngredient.md)
 - [CreateAllergen](./Models/CreateAllergen.md)
 - [CreateDish](./Models/CreateDish.md)
 - [CreateIngredient](./Models/CreateIngredient.md)
 - [CreateMeasure](./Models/CreateMeasure.md)
 - [Dish](./Models/Dish.md)
 - [DishCommonData](./Models/DishCommonData.md)
 - [DishDetails](./Models/DishDetails.md)
 - [DishDetails_allergens_inner](./Models/DishDetails_allergens_inner.md)
 - [DishDetails_ingredients_inner](./Models/DishDetails_ingredients_inner.md)
 - [DishSearchResult](./Models/DishSearchResult.md)
 - [DishSearchResultItem](./Models/DishSearchResultItem.md)
 - [Ingredient](./Models/Ingredient.md)
 - [IngredientCommonData](./Models/IngredientCommonData.md)
 - [IngredientDetails](./Models/IngredientDetails.md)
 - [Measure](./Models/Measure.md)
 - [MeasureDetails](./Models/MeasureDetails.md)
 - [MeasureDetails_allOf_ingredients](./Models/MeasureDetails_allOf_ingredients.md)
 - [Pagination](./Models/Pagination.md)
 - [SearchResult](./Models/SearchResult.md)
 - [UpdateAllergen](./Models/UpdateAllergen.md)
 - [UpdateDish](./Models/UpdateDish.md)
 - [UpdateIngredient](./Models/UpdateIngredient.md)
 - [UpdateMeasure](./Models/UpdateMeasure.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

All endpoints do not require authorization.
