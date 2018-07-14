# SkinApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180529/api/ws/v20180529*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getLicenses**](SkinApi.md#getLicenses) | **GET** /skn/license | Get licenses
[**getMaterials**](SkinApi.md#getMaterials) | **GET** /skn/material | Get materials
[**getShips**](SkinApi.md#getShips) | **GET** /skn/ship | Get ships
[**getSkins**](SkinApi.md#getSkins) | **GET** /skn/skin | Get skins


<a name="getLicenses"></a>
# **getLicenses**
> List&lt;SknLicense&gt; getLicenses(contid, maxresults, licenseTypeID, duration, skinID)

Get licenses



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.SkinApi;


SkinApi apiInstance = new SkinApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String licenseTypeID = "{ any: true }"; // String | License type ID selector
String duration = "{ any: true }"; // String | Duration selector
String skinID = "{ any: true }"; // String | Skin ID selector
try {
    List<SknLicense> result = apiInstance.getLicenses(contid, maxresults, licenseTypeID, duration, skinID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SkinApi#getLicenses");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **licenseTypeID** | **String**| License type ID selector | [optional] [default to { any: true }]
 **duration** | **String**| Duration selector | [optional] [default to { any: true }]
 **skinID** | **String**| Skin ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;SknLicense&gt;**](SknLicense.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getMaterials"></a>
# **getMaterials**
> List&lt;SknMaterial&gt; getMaterials(contid, maxresults, skinMaterialID, displayNameID, materialSetID)

Get materials



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.SkinApi;


SkinApi apiInstance = new SkinApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String skinMaterialID = "{ any: true }"; // String | Skin material ID selector
String displayNameID = "{ any: true }"; // String | Display name ID selector
String materialSetID = "{ any: true }"; // String | Material set ID selector
try {
    List<SknMaterial> result = apiInstance.getMaterials(contid, maxresults, skinMaterialID, displayNameID, materialSetID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SkinApi#getMaterials");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **skinMaterialID** | **String**| Skin material ID selector | [optional] [default to { any: true }]
 **displayNameID** | **String**| Display name ID selector | [optional] [default to { any: true }]
 **materialSetID** | **String**| Material set ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;SknMaterial&gt;**](SknMaterial.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getShips"></a>
# **getShips**
> List&lt;SknShip&gt; getShips(contid, maxresults, skinID, typeID)

Get ships



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.SkinApi;


SkinApi apiInstance = new SkinApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String skinID = "{ any: true }"; // String | Skin ID selector
String typeID = "{ any: true }"; // String | Type ID selector
try {
    List<SknShip> result = apiInstance.getShips(contid, maxresults, skinID, typeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SkinApi#getShips");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **skinID** | **String**| Skin ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;SknShip&gt;**](SknShip.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getSkins"></a>
# **getSkins**
> List&lt;SknSkin&gt; getSkins(contid, maxresults, skinID, internalName, skinMaterialID)

Get skins



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.SkinApi;


SkinApi apiInstance = new SkinApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String skinID = "{ any: true }"; // String | Skin ID selector
String internalName = "{ any: true }"; // String | Internal name selector
String skinMaterialID = "{ any: true }"; // String | Skin material ID selector
try {
    List<SknSkin> result = apiInstance.getSkins(contid, maxresults, skinID, internalName, skinMaterialID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SkinApi#getSkins");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **skinID** | **String**| Skin ID selector | [optional] [default to { any: true }]
 **internalName** | **String**| Internal name selector | [optional] [default to { any: true }]
 **skinMaterialID** | **String**| Skin material ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;SknSkin&gt;**](SknSkin.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

