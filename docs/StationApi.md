# StationApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180713/api/ws/v20180713*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getOperationServices**](StationApi.md#getOperationServices) | **GET** /sta/operation_service | Get operation services
[**getOperations**](StationApi.md#getOperations) | **GET** /sta/operation | Get operations
[**getServices**](StationApi.md#getServices) | **GET** /sta/service | Get services
[**getStationTypes**](StationApi.md#getStationTypes) | **GET** /sta/station_type | Get station types
[**getStations**](StationApi.md#getStations) | **GET** /sta/station | Get stations


<a name="getOperationServices"></a>
# **getOperationServices**
> List&lt;StaOperationService&gt; getOperationServices(contid, maxresults, operationID, serviceID)

Get operation services



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.StationApi;


StationApi apiInstance = new StationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String operationID = "{ any: true }"; // String | Operation ID selector
String serviceID = "{ any: true }"; // String | Service ID selector
try {
    List<StaOperationService> result = apiInstance.getOperationServices(contid, maxresults, operationID, serviceID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StationApi#getOperationServices");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **operationID** | **String**| Operation ID selector | [optional] [default to { any: true }]
 **serviceID** | **String**| Service ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;StaOperationService&gt;**](StaOperationService.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getOperations"></a>
# **getOperations**
> List&lt;StaOperation&gt; getOperations(contid, maxresults, operationID, activityID, amarrStationTypeID, border, caldariStationTypeID, corridor, description, fringe, gallenteStationTypeID, hub, joveStationTypeID, minmatarStationTypeID, operationName, ratio)

Get operations



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.StationApi;


StationApi apiInstance = new StationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String operationID = "{ any: true }"; // String | Operation ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String amarrStationTypeID = "{ any: true }"; // String | Amarr station type ID selector
String border = "{ any: true }"; // String | Border flag selector
String caldariStationTypeID = "{ any: true }"; // String | Caldari station type ID selector
String corridor = "{ any: true }"; // String | Corridor flag selector
String description = "{ any: true }"; // String | Description text selector
String fringe = "{ any: true }"; // String | Fringe flag selector
String gallenteStationTypeID = "{ any: true }"; // String | Gallente station type ID selector
String hub = "{ any: true }"; // String | Hub flag selector
String joveStationTypeID = "{ any: true }"; // String | Jove station type ID selector
String minmatarStationTypeID = "{ any: true }"; // String | Minmatar station type ID selector
String operationName = "{ any: true }"; // String | Operation name selector
String ratio = "{ any: true }"; // String | Ratio selector
try {
    List<StaOperation> result = apiInstance.getOperations(contid, maxresults, operationID, activityID, amarrStationTypeID, border, caldariStationTypeID, corridor, description, fringe, gallenteStationTypeID, hub, joveStationTypeID, minmatarStationTypeID, operationName, ratio);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StationApi#getOperations");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **operationID** | **String**| Operation ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **amarrStationTypeID** | **String**| Amarr station type ID selector | [optional] [default to { any: true }]
 **border** | **String**| Border flag selector | [optional] [default to { any: true }]
 **caldariStationTypeID** | **String**| Caldari station type ID selector | [optional] [default to { any: true }]
 **corridor** | **String**| Corridor flag selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **fringe** | **String**| Fringe flag selector | [optional] [default to { any: true }]
 **gallenteStationTypeID** | **String**| Gallente station type ID selector | [optional] [default to { any: true }]
 **hub** | **String**| Hub flag selector | [optional] [default to { any: true }]
 **joveStationTypeID** | **String**| Jove station type ID selector | [optional] [default to { any: true }]
 **minmatarStationTypeID** | **String**| Minmatar station type ID selector | [optional] [default to { any: true }]
 **operationName** | **String**| Operation name selector | [optional] [default to { any: true }]
 **ratio** | **String**| Ratio selector | [optional] [default to { any: true }]

### Return type

[**List&lt;StaOperation&gt;**](StaOperation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getServices"></a>
# **getServices**
> List&lt;StaService&gt; getServices(contid, maxresults, serviceID, description, serviceName)

Get services



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.StationApi;


StationApi apiInstance = new StationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String serviceID = "{ any: true }"; // String | Service ID selector
String description = "{ any: true }"; // String | Description text selector
String serviceName = "{ any: true }"; // String | Service name selector
try {
    List<StaService> result = apiInstance.getServices(contid, maxresults, serviceID, description, serviceName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StationApi#getServices");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **serviceID** | **String**| Service ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **serviceName** | **String**| Service name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;StaService&gt;**](StaService.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getStationTypes"></a>
# **getStationTypes**
> List&lt;StaStationType&gt; getStationTypes(contid, maxresults, stationTypeID, conquerable, dockEntryX, dockEntryY, dockEntryZ, dockOrientationX, dockOrientationY, dockOrientationZ, officeSlots, operationID, reprocessingEfficiency)

Get station types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.StationApi;


StationApi apiInstance = new StationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String stationTypeID = "{ any: true }"; // String | Station type ID selector
String conquerable = "{ any: true }"; // String | Conquerable flag selector
String dockEntryX = "{ any: true }"; // String | Dock entry X position selector
String dockEntryY = "{ any: true }"; // String | Dock entry Y position selector
String dockEntryZ = "{ any: true }"; // String | Dock entry Z position selector
String dockOrientationX = "{ any: true }"; // String | Dock orientation X position selector
String dockOrientationY = "{ any: true }"; // String | Dock orientation Y position selector
String dockOrientationZ = "{ any: true }"; // String | Dock orientation Z position selector
String officeSlots = "{ any: true }"; // String | Office slots selector
String operationID = "{ any: true }"; // String | Operation ID selector
String reprocessingEfficiency = "{ any: true }"; // String | Reprocessing efficiency selector
try {
    List<StaStationType> result = apiInstance.getStationTypes(contid, maxresults, stationTypeID, conquerable, dockEntryX, dockEntryY, dockEntryZ, dockOrientationX, dockOrientationY, dockOrientationZ, officeSlots, operationID, reprocessingEfficiency);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StationApi#getStationTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **stationTypeID** | **String**| Station type ID selector | [optional] [default to { any: true }]
 **conquerable** | **String**| Conquerable flag selector | [optional] [default to { any: true }]
 **dockEntryX** | **String**| Dock entry X position selector | [optional] [default to { any: true }]
 **dockEntryY** | **String**| Dock entry Y position selector | [optional] [default to { any: true }]
 **dockEntryZ** | **String**| Dock entry Z position selector | [optional] [default to { any: true }]
 **dockOrientationX** | **String**| Dock orientation X position selector | [optional] [default to { any: true }]
 **dockOrientationY** | **String**| Dock orientation Y position selector | [optional] [default to { any: true }]
 **dockOrientationZ** | **String**| Dock orientation Z position selector | [optional] [default to { any: true }]
 **officeSlots** | **String**| Office slots selector | [optional] [default to { any: true }]
 **operationID** | **String**| Operation ID selector | [optional] [default to { any: true }]
 **reprocessingEfficiency** | **String**| Reprocessing efficiency selector | [optional] [default to { any: true }]

### Return type

[**List&lt;StaStationType&gt;**](StaStationType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getStations"></a>
# **getStations**
> List&lt;StaStation&gt; getStations(contid, maxresults, stationID, constellationID, corporationID, dockingCostPerVolume, maxShipVolumeDockable, officeRentalCost, operationID, regionID, reprocessingEfficiency, reprocessingHangarFlag, reprocessingStationsTake, security, solarSystemID, stationName, stationTypeID, x, y, z)

Get stations



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.StationApi;


StationApi apiInstance = new StationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String stationID = "{ any: true }"; // String | Station ID selector
String constellationID = "{ any: true }"; // String | Constellation ID selector
String corporationID = "{ any: true }"; // String | Corporation ID selector
String dockingCostPerVolume = "{ any: true }"; // String | Docking cost per volume selector
String maxShipVolumeDockable = "{ any: true }"; // String | Max ship volume dockable selector
String officeRentalCost = "{ any: true }"; // String | Office rental cost selector
String operationID = "{ any: true }"; // String | Operation ID selector
String regionID = "{ any: true }"; // String | Region ID selector
String reprocessingEfficiency = "{ any: true }"; // String | Reprocessing efficiency selector
String reprocessingHangarFlag = "{ any: true }"; // String | Reprocessing hangar flag selector
String reprocessingStationsTake = "{ any: true }"; // String | Reprocessing stations take selector
String security = "{ any: true }"; // String | Security selector
String solarSystemID = "{ any: true }"; // String | Solar system ID selector
String stationName = "{ any: true }"; // String | Station name selector
String stationTypeID = "{ any: true }"; // String | Station type ID selector
String x = "{ any: true }"; // String | X position selector
String y = "{ any: true }"; // String | Y position selector
String z = "{ any: true }"; // String | Z position selector
try {
    List<StaStation> result = apiInstance.getStations(contid, maxresults, stationID, constellationID, corporationID, dockingCostPerVolume, maxShipVolumeDockable, officeRentalCost, operationID, regionID, reprocessingEfficiency, reprocessingHangarFlag, reprocessingStationsTake, security, solarSystemID, stationName, stationTypeID, x, y, z);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StationApi#getStations");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **stationID** | **String**| Station ID selector | [optional] [default to { any: true }]
 **constellationID** | **String**| Constellation ID selector | [optional] [default to { any: true }]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]
 **dockingCostPerVolume** | **String**| Docking cost per volume selector | [optional] [default to { any: true }]
 **maxShipVolumeDockable** | **String**| Max ship volume dockable selector | [optional] [default to { any: true }]
 **officeRentalCost** | **String**| Office rental cost selector | [optional] [default to { any: true }]
 **operationID** | **String**| Operation ID selector | [optional] [default to { any: true }]
 **regionID** | **String**| Region ID selector | [optional] [default to { any: true }]
 **reprocessingEfficiency** | **String**| Reprocessing efficiency selector | [optional] [default to { any: true }]
 **reprocessingHangarFlag** | **String**| Reprocessing hangar flag selector | [optional] [default to { any: true }]
 **reprocessingStationsTake** | **String**| Reprocessing stations take selector | [optional] [default to { any: true }]
 **security** | **String**| Security selector | [optional] [default to { any: true }]
 **solarSystemID** | **String**| Solar system ID selector | [optional] [default to { any: true }]
 **stationName** | **String**| Station name selector | [optional] [default to { any: true }]
 **stationTypeID** | **String**| Station type ID selector | [optional] [default to { any: true }]
 **x** | **String**| X position selector | [optional] [default to { any: true }]
 **y** | **String**| Y position selector | [optional] [default to { any: true }]
 **z** | **String**| Z position selector | [optional] [default to { any: true }]

### Return type

[**List&lt;StaStation&gt;**](StaStation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

