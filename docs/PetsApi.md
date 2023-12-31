# SwaggerPetstore.PetsApi

All URIs are relative to *http://petstore.swagger.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPets**](PetsApi.md#createPets) | **POST** /pets | Create a pet
[**listPets**](PetsApi.md#listPets) | **GET** /pets | List all pets
[**showPetById**](PetsApi.md#showPetById) | **GET** /pets/{petId} | Info for a specific pet



## createPets

> createPets()

Create a pet

### Example

```javascript
import SwaggerPetstore from 'swagger_petstore';

let apiInstance = new SwaggerPetstore.PetsApi();
apiInstance.createPets((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPets

> [Pet] listPets(opts)

List all pets

### Example

```javascript
import SwaggerPetstore from 'swagger_petstore';

let apiInstance = new SwaggerPetstore.PetsApi();
let opts = {
  'limit': 56 // Number | How many items to return at one time (max 100)
};
apiInstance.listPets(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **Number**| How many items to return at one time (max 100) | [optional] 

### Return type

[**[Pet]**](Pet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## showPetById

> Pet showPetById(petId)

Info for a specific pet

### Example

```javascript
import SwaggerPetstore from 'swagger_petstore';

let apiInstance = new SwaggerPetstore.PetsApi();
let petId = "petId_example"; // String | The id of the pet to retrieve
apiInstance.showPetById(petId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **petId** | **String**| The id of the pet to retrieve | 

### Return type

[**Pet**](Pet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

