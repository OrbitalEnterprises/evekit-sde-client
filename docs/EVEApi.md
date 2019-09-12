# EVEApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20190625/api/ws/v20190625*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getGraphics**](EVEApi.md#getGraphics) | **GET** /eve/graphic | Get graphics
[**getIcons**](EVEApi.md#getIcons) | **GET** /eve/icon | Get icons
[**getUnits**](EVEApi.md#getUnits) | **GET** /eve/unit | Get units


<a name="getGraphics"></a>
# **getGraphics**
> List&lt;EveGraphic&gt; getGraphics(contid, maxresults, graphicID, sofFactionName, graphicFile, sofHullName, sofRaceName, description)

Get graphics



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.EVEApi;


EVEApi apiInstance = new EVEApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String graphicID = "{ any: true }"; // String | Graphic ID selector
String sofFactionName = "{ any: true }"; // String | Faction name selector
String graphicFile = "{ any: true }"; // String | Graphic file selector
String sofHullName = "{ any: true }"; // String | Hull name selector
String sofRaceName = "{ any: true }"; // String | Race name selector
String description = "{ any: true }"; // String | Description selector
try {
    List<EveGraphic> result = apiInstance.getGraphics(contid, maxresults, graphicID, sofFactionName, graphicFile, sofHullName, sofRaceName, description);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EVEApi#getGraphics");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **graphicID** | **String**| Graphic ID selector | [optional] [default to { any: true }]
 **sofFactionName** | **String**| Faction name selector | [optional] [default to { any: true }]
 **graphicFile** | **String**| Graphic file selector | [optional] [default to { any: true }]
 **sofHullName** | **String**| Hull name selector | [optional] [default to { any: true }]
 **sofRaceName** | **String**| Race name selector | [optional] [default to { any: true }]
 **description** | **String**| Description selector | [optional] [default to { any: true }]

### Return type

[**List&lt;EveGraphic&gt;**](EveGraphic.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getIcons"></a>
# **getIcons**
> List&lt;EveIcon&gt; getIcons(contid, maxresults, iconID, description, iconFile)

Get icons



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.EVEApi;


EVEApi apiInstance = new EVEApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String iconID = "{ any: true }"; // String | Icon ID selector
String description = "{ any: true }"; // String | Description text selector
String iconFile = "{ any: true }"; // String | Icon file selector
try {
    List<EveIcon> result = apiInstance.getIcons(contid, maxresults, iconID, description, iconFile);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EVEApi#getIcons");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **iconFile** | **String**| Icon file selector | [optional] [default to { any: true }]

### Return type

[**List&lt;EveIcon&gt;**](EveIcon.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getUnits"></a>
# **getUnits**
> List&lt;EveUnit&gt; getUnits(contid, maxresults, unitID, description, displayName, unitName)

Get units



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.EVEApi;


EVEApi apiInstance = new EVEApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String unitID = "{ any: true }"; // String | Unit ID selector
String description = "{ any: true }"; // String | Description text selector
String displayName = "{ any: true }"; // String | Display name selector
String unitName = "{ any: true }"; // String | Unit name selector
try {
    List<EveUnit> result = apiInstance.getUnits(contid, maxresults, unitID, description, displayName, unitName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EVEApi#getUnits");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **unitID** | **String**| Unit ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **displayName** | **String**| Display name selector | [optional] [default to { any: true }]
 **unitName** | **String**| Unit name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;EveUnit&gt;**](EveUnit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

