# PlanetApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20190219/api/ws/v20190219*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getSchematicPinMaps**](PlanetApi.md#getSchematicPinMaps) | **GET** /plt/schematic_pin_map | Get schematic pin maps
[**getSchematicTypeMaps**](PlanetApi.md#getSchematicTypeMaps) | **GET** /plt/schematic_type_map | Get schematic type maps
[**getSchematics**](PlanetApi.md#getSchematics) | **GET** /plt/schematic | Get schematics


<a name="getSchematicPinMaps"></a>
# **getSchematicPinMaps**
> List&lt;PltSchematicsPinMap&gt; getSchematicPinMaps(contid, maxresults, schematicID, pinTypeID)

Get schematic pin maps



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.PlanetApi;


PlanetApi apiInstance = new PlanetApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String schematicID = "{ any: true }"; // String | Schematic ID selector
String pinTypeID = "{ any: true }"; // String | Pin type ID selector
try {
    List<PltSchematicsPinMap> result = apiInstance.getSchematicPinMaps(contid, maxresults, schematicID, pinTypeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PlanetApi#getSchematicPinMaps");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **schematicID** | **String**| Schematic ID selector | [optional] [default to { any: true }]
 **pinTypeID** | **String**| Pin type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;PltSchematicsPinMap&gt;**](PltSchematicsPinMap.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getSchematicTypeMaps"></a>
# **getSchematicTypeMaps**
> List&lt;PltSchematicsTypeMap&gt; getSchematicTypeMaps(contid, maxresults, schematicID, typeID, isInput, quantity)

Get schematic type maps



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.PlanetApi;


PlanetApi apiInstance = new PlanetApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String schematicID = "{ any: true }"; // String | Schematic ID selector
String typeID = "{ any: true }"; // String | Type ID selector
String isInput = "{ any: true }"; // String | Is input flag selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<PltSchematicsTypeMap> result = apiInstance.getSchematicTypeMaps(contid, maxresults, schematicID, typeID, isInput, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PlanetApi#getSchematicTypeMaps");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **schematicID** | **String**| Schematic ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **isInput** | **String**| Is input flag selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;PltSchematicsTypeMap&gt;**](PltSchematicsTypeMap.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getSchematics"></a>
# **getSchematics**
> List&lt;PltSchematic&gt; getSchematics(contid, maxresults, schematicID, cycleTime, schematicName)

Get schematics



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.PlanetApi;


PlanetApi apiInstance = new PlanetApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String schematicID = "{ any: true }"; // String | Schematic ID selector
String cycleTime = "{ any: true }"; // String | Cycle time selector
String schematicName = "{ any: true }"; // String | Schematic name selector
try {
    List<PltSchematic> result = apiInstance.getSchematics(contid, maxresults, schematicID, cycleTime, schematicName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PlanetApi#getSchematics");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **schematicID** | **String**| Schematic ID selector | [optional] [default to { any: true }]
 **cycleTime** | **String**| Cycle time selector | [optional] [default to { any: true }]
 **schematicName** | **String**| Schematic name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;PltSchematic&gt;**](PltSchematic.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

