# RAMApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180917/api/ws/v20180917*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAssemblyLineStations**](RAMApi.md#getAssemblyLineStations) | **GET** /ram/assembly_line_station | Get assembly line stations
[**getAssemblyLineTypeDetailsPerCategory**](RAMApi.md#getAssemblyLineTypeDetailsPerCategory) | **GET** /ram/assembly_line_type_detail_per_category | Get assembly line type details per category
[**getAssemblyLineTypeDetailsPerGroup**](RAMApi.md#getAssemblyLineTypeDetailsPerGroup) | **GET** /ram/assembly_line_type_detail_per_group | Get assembly line type details per group
[**getAssemblyLineTypes**](RAMApi.md#getAssemblyLineTypes) | **GET** /ram/assembly_line_type | Get assembly line types
[**getInstallationTypeContents**](RAMApi.md#getInstallationTypeContents) | **GET** /ram/installation_type_content | Get installation type contents
[**getRAMActivities**](RAMApi.md#getRAMActivities) | **GET** /ram/activity | Get activities


<a name="getAssemblyLineStations"></a>
# **getAssemblyLineStations**
> List&lt;RamAssemblyLineStation&gt; getAssemblyLineStations(contid, maxresults, stationID, assemblyLineTypeID, ownerID, quantity, regionID, solarSystemID, stationTypeID)

Get assembly line stations



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.RAMApi;


RAMApi apiInstance = new RAMApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String stationID = "{ any: true }"; // String | Station ID selector
String assemblyLineTypeID = "{ any: true }"; // String | Assembly line type ID selector
String ownerID = "{ any: true }"; // String | Owner ID selector
String quantity = "{ any: true }"; // String | Quantity selector
String regionID = "{ any: true }"; // String | Region ID selector
String solarSystemID = "{ any: true }"; // String | Solary system ID selector
String stationTypeID = "{ any: true }"; // String | Station type ID selector
try {
    List<RamAssemblyLineStation> result = apiInstance.getAssemblyLineStations(contid, maxresults, stationID, assemblyLineTypeID, ownerID, quantity, regionID, solarSystemID, stationTypeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RAMApi#getAssemblyLineStations");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **stationID** | **String**| Station ID selector | [optional] [default to { any: true }]
 **assemblyLineTypeID** | **String**| Assembly line type ID selector | [optional] [default to { any: true }]
 **ownerID** | **String**| Owner ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]
 **regionID** | **String**| Region ID selector | [optional] [default to { any: true }]
 **solarSystemID** | **String**| Solary system ID selector | [optional] [default to { any: true }]
 **stationTypeID** | **String**| Station type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;RamAssemblyLineStation&gt;**](RamAssemblyLineStation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getAssemblyLineTypeDetailsPerCategory"></a>
# **getAssemblyLineTypeDetailsPerCategory**
> List&lt;RamAssemblyLineTypeDetailPerCategory&gt; getAssemblyLineTypeDetailsPerCategory(contid, maxresults, assemblyLineTypeID, categoryID, costMultiplier, materialMultiplier, timeMultiplier)

Get assembly line type details per category



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.RAMApi;


RAMApi apiInstance = new RAMApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String assemblyLineTypeID = "{ any: true }"; // String | Assembly line type ID selector
String categoryID = "{ any: true }"; // String | Category ID selector
String costMultiplier = "{ any: true }"; // String | Cost multiplier selector
String materialMultiplier = "{ any: true }"; // String | Material multiplier selector
String timeMultiplier = "{ any: true }"; // String | Time multiplier selector
try {
    List<RamAssemblyLineTypeDetailPerCategory> result = apiInstance.getAssemblyLineTypeDetailsPerCategory(contid, maxresults, assemblyLineTypeID, categoryID, costMultiplier, materialMultiplier, timeMultiplier);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RAMApi#getAssemblyLineTypeDetailsPerCategory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **assemblyLineTypeID** | **String**| Assembly line type ID selector | [optional] [default to { any: true }]
 **categoryID** | **String**| Category ID selector | [optional] [default to { any: true }]
 **costMultiplier** | **String**| Cost multiplier selector | [optional] [default to { any: true }]
 **materialMultiplier** | **String**| Material multiplier selector | [optional] [default to { any: true }]
 **timeMultiplier** | **String**| Time multiplier selector | [optional] [default to { any: true }]

### Return type

[**List&lt;RamAssemblyLineTypeDetailPerCategory&gt;**](RamAssemblyLineTypeDetailPerCategory.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getAssemblyLineTypeDetailsPerGroup"></a>
# **getAssemblyLineTypeDetailsPerGroup**
> List&lt;RamAssemblyLineTypeDetailPerGroup&gt; getAssemblyLineTypeDetailsPerGroup(contid, maxresults, assemblyLineTypeID, groupID, costMultiplier, materialMultiplier, timeMultiplier)

Get assembly line type details per group



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.RAMApi;


RAMApi apiInstance = new RAMApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String assemblyLineTypeID = "{ any: true }"; // String | Assembly line type ID selector
String groupID = "{ any: true }"; // String | Group ID selector
String costMultiplier = "{ any: true }"; // String | Cost multiplier selector
String materialMultiplier = "{ any: true }"; // String | Material multiplier selector
String timeMultiplier = "{ any: true }"; // String | Time multiplier selector
try {
    List<RamAssemblyLineTypeDetailPerGroup> result = apiInstance.getAssemblyLineTypeDetailsPerGroup(contid, maxresults, assemblyLineTypeID, groupID, costMultiplier, materialMultiplier, timeMultiplier);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RAMApi#getAssemblyLineTypeDetailsPerGroup");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **assemblyLineTypeID** | **String**| Assembly line type ID selector | [optional] [default to { any: true }]
 **groupID** | **String**| Group ID selector | [optional] [default to { any: true }]
 **costMultiplier** | **String**| Cost multiplier selector | [optional] [default to { any: true }]
 **materialMultiplier** | **String**| Material multiplier selector | [optional] [default to { any: true }]
 **timeMultiplier** | **String**| Time multiplier selector | [optional] [default to { any: true }]

### Return type

[**List&lt;RamAssemblyLineTypeDetailPerGroup&gt;**](RamAssemblyLineTypeDetailPerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getAssemblyLineTypes"></a>
# **getAssemblyLineTypes**
> List&lt;RamAssemblyLineType&gt; getAssemblyLineTypes(contid, maxresults, assemblyLineTypeID, activityID, assemblyLineTypeName, baseCostMultiplier, baseMaterialMultiplier, baseTimeMultiplier, description, minCostPerHour, volume)

Get assembly line types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.RAMApi;


RAMApi apiInstance = new RAMApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String assemblyLineTypeID = "{ any: true }"; // String | Assembly line type ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String assemblyLineTypeName = "{ any: true }"; // String | Assembly line type name selector
String baseCostMultiplier = "{ any: true }"; // String | Base cost multiplier selector
String baseMaterialMultiplier = "{ any: true }"; // String | Base material multiplier selector
String baseTimeMultiplier = "{ any: true }"; // String | Base time multiplier selector
String description = "{ any: true }"; // String | Description text selector
String minCostPerHour = "{ any: true }"; // String | Minimum cost per hour selector
String volume = "{ any: true }"; // String | Volume selector
try {
    List<RamAssemblyLineType> result = apiInstance.getAssemblyLineTypes(contid, maxresults, assemblyLineTypeID, activityID, assemblyLineTypeName, baseCostMultiplier, baseMaterialMultiplier, baseTimeMultiplier, description, minCostPerHour, volume);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RAMApi#getAssemblyLineTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **assemblyLineTypeID** | **String**| Assembly line type ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **assemblyLineTypeName** | **String**| Assembly line type name selector | [optional] [default to { any: true }]
 **baseCostMultiplier** | **String**| Base cost multiplier selector | [optional] [default to { any: true }]
 **baseMaterialMultiplier** | **String**| Base material multiplier selector | [optional] [default to { any: true }]
 **baseTimeMultiplier** | **String**| Base time multiplier selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **minCostPerHour** | **String**| Minimum cost per hour selector | [optional] [default to { any: true }]
 **volume** | **String**| Volume selector | [optional] [default to { any: true }]

### Return type

[**List&lt;RamAssemblyLineType&gt;**](RamAssemblyLineType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getInstallationTypeContents"></a>
# **getInstallationTypeContents**
> List&lt;RamInstallationTypeContent&gt; getInstallationTypeContents(contid, maxresults, installationTypeID, assemblyLineTypeID, quantity)

Get installation type contents



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.RAMApi;


RAMApi apiInstance = new RAMApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String installationTypeID = "{ any: true }"; // String | Installation type ID selector
String assemblyLineTypeID = "{ any: true }"; // String | Assembly line type ID selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<RamInstallationTypeContent> result = apiInstance.getInstallationTypeContents(contid, maxresults, installationTypeID, assemblyLineTypeID, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RAMApi#getInstallationTypeContents");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **installationTypeID** | **String**| Installation type ID selector | [optional] [default to { any: true }]
 **assemblyLineTypeID** | **String**| Assembly line type ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;RamInstallationTypeContent&gt;**](RamInstallationTypeContent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getRAMActivities"></a>
# **getRAMActivities**
> List&lt;RamActivity&gt; getRAMActivities(contid, maxresults, activityID, activityName, description, iconNo, published)

Get activities



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.RAMApi;


RAMApi apiInstance = new RAMApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String activityID = "{ any: true }"; // String | Activity ID selector
String activityName = "{ any: true }"; // String | Activity name selector
String description = "{ any: true }"; // String | Description text selector
String iconNo = "{ any: true }"; // String | Icon number selector
String published = "{ any: true }"; // String | Published flag selector
try {
    List<RamActivity> result = apiInstance.getRAMActivities(contid, maxresults, activityID, activityName, description, iconNo, published);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RAMApi#getRAMActivities");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **activityName** | **String**| Activity name selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **iconNo** | **String**| Icon number selector | [optional] [default to { any: true }]
 **published** | **String**| Published flag selector | [optional] [default to { any: true }]

### Return type

[**List&lt;RamActivity&gt;**](RamActivity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

