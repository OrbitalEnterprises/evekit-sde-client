# MapApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20190516/api/ws/v20190516*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCelestialStatistics**](MapApi.md#getCelestialStatistics) | **GET** /map/celestial_statistic | Get celestial statistics
[**getConstellationJumps**](MapApi.md#getConstellationJumps) | **GET** /map/constellation_jump | Get constellation jumps
[**getConstellations**](MapApi.md#getConstellations) | **GET** /map/constellation | Get constellations
[**getDenormalization**](MapApi.md#getDenormalization) | **GET** /map/denormalize | Get denormalization
[**getJumps**](MapApi.md#getJumps) | **GET** /map/jump | Get jumps
[**getLocationScenes**](MapApi.md#getLocationScenes) | **GET** /map/location_scene | Get location scenes
[**getLocationWormholeClasses**](MapApi.md#getLocationWormholeClasses) | **GET** /map/location_wormhole_class | Get location wormhole classes
[**getRegionJumps**](MapApi.md#getRegionJumps) | **GET** /map/region_jump | Get region jumps
[**getRegions**](MapApi.md#getRegions) | **GET** /map/region | Get regions
[**getSolarSystemJumps**](MapApi.md#getSolarSystemJumps) | **GET** /map/solar_system_jump | Get solar system jumps
[**getSolarSystems**](MapApi.md#getSolarSystems) | **GET** /map/solar_system | Get solar systems
[**getUniverses**](MapApi.md#getUniverses) | **GET** /map/universe | Get universes


<a name="getCelestialStatistics"></a>
# **getCelestialStatistics**
> List&lt;MapCelestialStatistic&gt; getCelestialStatistics(contid, maxresults, celestialID, age, density, eccentricity, escapeVelocity, fragmented, life, locked, luminosity, mass, massDust, massGas, orbitPeriod, orbitRadius, pressure, radius, rotationRate, spectralClass, surfaceGravity, temperature)

Get celestial statistics



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String celestialID = "{ any: true }"; // String | Celestial ID selector
String age = "{ any: true }"; // String | Age selector
String density = "{ any: true }"; // String | Density selector
String eccentricity = "{ any: true }"; // String | Eccentricity selector
String escapeVelocity = "{ any: true }"; // String | Escape velocity selector
String fragmented = "{ any: true }"; // String | Fragmented flag selector
String life = "{ any: true }"; // String | Life flag selector
String locked = "{ any: true }"; // String | Locked flag selector
String luminosity = "{ any: true }"; // String | Luminosity selector
String mass = "{ any: true }"; // String | Mass selector
String massDust = "{ any: true }"; // String | Mass dust selector
String massGas = "{ any: true }"; // String | Mass gas selector
String orbitPeriod = "{ any: true }"; // String | Orbit period selector
String orbitRadius = "{ any: true }"; // String | Orbit radius selector
String pressure = "{ any: true }"; // String | Pressure selector
String radius = "{ any: true }"; // String | Radius selector
String rotationRate = "{ any: true }"; // String | Rotation rate selector
String spectralClass = "{ any: true }"; // String | Spectral class selector
String surfaceGravity = "{ any: true }"; // String | Surface gravity selector
String temperature = "{ any: true }"; // String | Temperature selector
try {
    List<MapCelestialStatistic> result = apiInstance.getCelestialStatistics(contid, maxresults, celestialID, age, density, eccentricity, escapeVelocity, fragmented, life, locked, luminosity, mass, massDust, massGas, orbitPeriod, orbitRadius, pressure, radius, rotationRate, spectralClass, surfaceGravity, temperature);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getCelestialStatistics");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **celestialID** | **String**| Celestial ID selector | [optional] [default to { any: true }]
 **age** | **String**| Age selector | [optional] [default to { any: true }]
 **density** | **String**| Density selector | [optional] [default to { any: true }]
 **eccentricity** | **String**| Eccentricity selector | [optional] [default to { any: true }]
 **escapeVelocity** | **String**| Escape velocity selector | [optional] [default to { any: true }]
 **fragmented** | **String**| Fragmented flag selector | [optional] [default to { any: true }]
 **life** | **String**| Life flag selector | [optional] [default to { any: true }]
 **locked** | **String**| Locked flag selector | [optional] [default to { any: true }]
 **luminosity** | **String**| Luminosity selector | [optional] [default to { any: true }]
 **mass** | **String**| Mass selector | [optional] [default to { any: true }]
 **massDust** | **String**| Mass dust selector | [optional] [default to { any: true }]
 **massGas** | **String**| Mass gas selector | [optional] [default to { any: true }]
 **orbitPeriod** | **String**| Orbit period selector | [optional] [default to { any: true }]
 **orbitRadius** | **String**| Orbit radius selector | [optional] [default to { any: true }]
 **pressure** | **String**| Pressure selector | [optional] [default to { any: true }]
 **radius** | **String**| Radius selector | [optional] [default to { any: true }]
 **rotationRate** | **String**| Rotation rate selector | [optional] [default to { any: true }]
 **spectralClass** | **String**| Spectral class selector | [optional] [default to { any: true }]
 **surfaceGravity** | **String**| Surface gravity selector | [optional] [default to { any: true }]
 **temperature** | **String**| Temperature selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapCelestialStatistic&gt;**](MapCelestialStatistic.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getConstellationJumps"></a>
# **getConstellationJumps**
> List&lt;MapConstellationJump&gt; getConstellationJumps(contid, maxresults, fromConstellationID, toConstellationID, fromRegionID, toRegionID)

Get constellation jumps



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String fromConstellationID = "{ any: true }"; // String | From constellation ID selector
String toConstellationID = "{ any: true }"; // String | To constellation ID selector
String fromRegionID = "{ any: true }"; // String | From region ID selector
String toRegionID = "{ any: true }"; // String | To region ID selector
try {
    List<MapConstellationJump> result = apiInstance.getConstellationJumps(contid, maxresults, fromConstellationID, toConstellationID, fromRegionID, toRegionID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getConstellationJumps");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **fromConstellationID** | **String**| From constellation ID selector | [optional] [default to { any: true }]
 **toConstellationID** | **String**| To constellation ID selector | [optional] [default to { any: true }]
 **fromRegionID** | **String**| From region ID selector | [optional] [default to { any: true }]
 **toRegionID** | **String**| To region ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapConstellationJump&gt;**](MapConstellationJump.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getConstellations"></a>
# **getConstellations**
> List&lt;MapConstellation&gt; getConstellations(contid, maxresults, constellationID, constellationName, factionID, radius, regionID, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin)

Get constellations



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String constellationID = "{ any: true }"; // String | Constellation ID selector
String constellationName = "{ any: true }"; // String | Constellation name selector
String factionID = "{ any: true }"; // String | Faction ID selector
String radius = "{ any: true }"; // String | Radius selector
String regionID = "{ any: true }"; // String | Region ID selector
String x = "{ any: true }"; // String | X position selector
String xMax = "{ any: true }"; // String | Max X extent selector
String xMin = "{ any: true }"; // String | Min X extent selector
String y = "{ any: true }"; // String | Y position selector
String yMax = "{ any: true }"; // String | Max Y extent selector
String yMin = "{ any: true }"; // String | Min Y extent selector
String z = "{ any: true }"; // String | Z position selector
String zMax = "{ any: true }"; // String | Max Z extent selector
String zMin = "{ any: true }"; // String | Min Z extent selector
try {
    List<MapConstellation> result = apiInstance.getConstellations(contid, maxresults, constellationID, constellationName, factionID, radius, regionID, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getConstellations");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **constellationID** | **String**| Constellation ID selector | [optional] [default to { any: true }]
 **constellationName** | **String**| Constellation name selector | [optional] [default to { any: true }]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]
 **radius** | **String**| Radius selector | [optional] [default to { any: true }]
 **regionID** | **String**| Region ID selector | [optional] [default to { any: true }]
 **x** | **String**| X position selector | [optional] [default to { any: true }]
 **xMax** | **String**| Max X extent selector | [optional] [default to { any: true }]
 **xMin** | **String**| Min X extent selector | [optional] [default to { any: true }]
 **y** | **String**| Y position selector | [optional] [default to { any: true }]
 **yMax** | **String**| Max Y extent selector | [optional] [default to { any: true }]
 **yMin** | **String**| Min Y extent selector | [optional] [default to { any: true }]
 **z** | **String**| Z position selector | [optional] [default to { any: true }]
 **zMax** | **String**| Max Z extent selector | [optional] [default to { any: true }]
 **zMin** | **String**| Min Z extent selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapConstellation&gt;**](MapConstellation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getDenormalization"></a>
# **getDenormalization**
> List&lt;MapDenormalize&gt; getDenormalization(contid, maxresults, itemID, celestialIndex, constellationID, groupID, itemName, orbitID, orbitIndex, radius, regionID, security, solarSystemID, typeID, x, y, z)

Get denormalization



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String itemID = "{ any: true }"; // String | Item ID selector
String celestialIndex = "{ any: true }"; // String | Celestial index selector
String constellationID = "{ any: true }"; // String | Constellation ID selector
String groupID = "{ any: true }"; // String | Group ID selector
String itemName = "{ any: true }"; // String | Item name selector
String orbitID = "{ any: true }"; // String | Orbit ID selector
String orbitIndex = "{ any: true }"; // String | Orbit index selector
String radius = "{ any: true }"; // String | Radius selector
String regionID = "{ any: true }"; // String | Region ID selector
String security = "{ any: true }"; // String | Security selector
String solarSystemID = "{ any: true }"; // String | Solar system ID selector
String typeID = "{ any: true }"; // String | Type ID selector
String x = "{ any: true }"; // String | X position selector
String y = "{ any: true }"; // String | Y position selector
String z = "{ any: true }"; // String | Z position selector
try {
    List<MapDenormalize> result = apiInstance.getDenormalization(contid, maxresults, itemID, celestialIndex, constellationID, groupID, itemName, orbitID, orbitIndex, radius, regionID, security, solarSystemID, typeID, x, y, z);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getDenormalization");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **itemID** | **String**| Item ID selector | [optional] [default to { any: true }]
 **celestialIndex** | **String**| Celestial index selector | [optional] [default to { any: true }]
 **constellationID** | **String**| Constellation ID selector | [optional] [default to { any: true }]
 **groupID** | **String**| Group ID selector | [optional] [default to { any: true }]
 **itemName** | **String**| Item name selector | [optional] [default to { any: true }]
 **orbitID** | **String**| Orbit ID selector | [optional] [default to { any: true }]
 **orbitIndex** | **String**| Orbit index selector | [optional] [default to { any: true }]
 **radius** | **String**| Radius selector | [optional] [default to { any: true }]
 **regionID** | **String**| Region ID selector | [optional] [default to { any: true }]
 **security** | **String**| Security selector | [optional] [default to { any: true }]
 **solarSystemID** | **String**| Solar system ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **x** | **String**| X position selector | [optional] [default to { any: true }]
 **y** | **String**| Y position selector | [optional] [default to { any: true }]
 **z** | **String**| Z position selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapDenormalize&gt;**](MapDenormalize.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getJumps"></a>
# **getJumps**
> List&lt;MapJump&gt; getJumps(contid, maxresults, stargateID, destinationID)

Get jumps



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String stargateID = "{ any: true }"; // String | Stargate ID selector
String destinationID = "{ any: true }"; // String | Destination ID selector
try {
    List<MapJump> result = apiInstance.getJumps(contid, maxresults, stargateID, destinationID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getJumps");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **stargateID** | **String**| Stargate ID selector | [optional] [default to { any: true }]
 **destinationID** | **String**| Destination ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapJump&gt;**](MapJump.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getLocationScenes"></a>
# **getLocationScenes**
> List&lt;MapLocationScene&gt; getLocationScenes(contid, maxresults, locationID, graphicID)

Get location scenes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String locationID = "{ any: true }"; // String | Location ID selector
String graphicID = "{ any: true }"; // String | Graphic ID selector
try {
    List<MapLocationScene> result = apiInstance.getLocationScenes(contid, maxresults, locationID, graphicID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getLocationScenes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **locationID** | **String**| Location ID selector | [optional] [default to { any: true }]
 **graphicID** | **String**| Graphic ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapLocationScene&gt;**](MapLocationScene.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getLocationWormholeClasses"></a>
# **getLocationWormholeClasses**
> List&lt;MapLocationWormholeClass&gt; getLocationWormholeClasses(contid, maxresults, locationID, wormholeClassID)

Get location wormhole classes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String locationID = "{ any: true }"; // String | Location ID selector
String wormholeClassID = "{ any: true }"; // String | Wormhole class ID selector
try {
    List<MapLocationWormholeClass> result = apiInstance.getLocationWormholeClasses(contid, maxresults, locationID, wormholeClassID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getLocationWormholeClasses");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **locationID** | **String**| Location ID selector | [optional] [default to { any: true }]
 **wormholeClassID** | **String**| Wormhole class ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapLocationWormholeClass&gt;**](MapLocationWormholeClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getRegionJumps"></a>
# **getRegionJumps**
> List&lt;MapRegionJump&gt; getRegionJumps(contid, maxresults, fromRegionID, toRegionID)

Get region jumps



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String fromRegionID = "{ any: true }"; // String | From region ID selector
String toRegionID = "{ any: true }"; // String | To region ID selector
try {
    List<MapRegionJump> result = apiInstance.getRegionJumps(contid, maxresults, fromRegionID, toRegionID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getRegionJumps");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **fromRegionID** | **String**| From region ID selector | [optional] [default to { any: true }]
 **toRegionID** | **String**| To region ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapRegionJump&gt;**](MapRegionJump.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getRegions"></a>
# **getRegions**
> List&lt;MapRegion&gt; getRegions(contid, maxresults, regionID, factionID, radius, regionName, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin)

Get regions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String regionID = "{ any: true }"; // String | Region ID selector
String factionID = "{ any: true }"; // String | Faction ID selector
String radius = "{ any: true }"; // String | Radius selector
String regionName = "{ any: true }"; // String | Region name selector
String x = "{ any: true }"; // String | X position selector
String xMax = "{ any: true }"; // String | Max X extent selector
String xMin = "{ any: true }"; // String | Min X extent selector
String y = "{ any: true }"; // String | Y position selector
String yMax = "{ any: true }"; // String | Max Y extent selector
String yMin = "{ any: true }"; // String | Min Y extent selector
String z = "{ any: true }"; // String | Z position selector
String zMax = "{ any: true }"; // String | Max Z extent selector
String zMin = "{ any: true }"; // String | Min Z extent selector
try {
    List<MapRegion> result = apiInstance.getRegions(contid, maxresults, regionID, factionID, radius, regionName, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getRegions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **regionID** | **String**| Region ID selector | [optional] [default to { any: true }]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]
 **radius** | **String**| Radius selector | [optional] [default to { any: true }]
 **regionName** | **String**| Region name selector | [optional] [default to { any: true }]
 **x** | **String**| X position selector | [optional] [default to { any: true }]
 **xMax** | **String**| Max X extent selector | [optional] [default to { any: true }]
 **xMin** | **String**| Min X extent selector | [optional] [default to { any: true }]
 **y** | **String**| Y position selector | [optional] [default to { any: true }]
 **yMax** | **String**| Max Y extent selector | [optional] [default to { any: true }]
 **yMin** | **String**| Min Y extent selector | [optional] [default to { any: true }]
 **z** | **String**| Z position selector | [optional] [default to { any: true }]
 **zMax** | **String**| Max Z extent selector | [optional] [default to { any: true }]
 **zMin** | **String**| Min Z extent selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapRegion&gt;**](MapRegion.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getSolarSystemJumps"></a>
# **getSolarSystemJumps**
> List&lt;MapSolarSystemJump&gt; getSolarSystemJumps(contid, maxresults, fromSolarSystemID, toSolarSystemID, fromConstellationID, fromRegionID, toConstellationID, toRegionID)

Get solar system jumps



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String fromSolarSystemID = "{ any: true }"; // String | Source solar system ID selector
String toSolarSystemID = "{ any: true }"; // String | Destination solar system ID selector
String fromConstellationID = "{ any: true }"; // String | Source constellation ID selector
String fromRegionID = "{ any: true }"; // String | Source region ID selector
String toConstellationID = "{ any: true }"; // String | Destination constellation ID selector
String toRegionID = "{ any: true }"; // String | Destination region ID selector
try {
    List<MapSolarSystemJump> result = apiInstance.getSolarSystemJumps(contid, maxresults, fromSolarSystemID, toSolarSystemID, fromConstellationID, fromRegionID, toConstellationID, toRegionID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getSolarSystemJumps");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **fromSolarSystemID** | **String**| Source solar system ID selector | [optional] [default to { any: true }]
 **toSolarSystemID** | **String**| Destination solar system ID selector | [optional] [default to { any: true }]
 **fromConstellationID** | **String**| Source constellation ID selector | [optional] [default to { any: true }]
 **fromRegionID** | **String**| Source region ID selector | [optional] [default to { any: true }]
 **toConstellationID** | **String**| Destination constellation ID selector | [optional] [default to { any: true }]
 **toRegionID** | **String**| Destination region ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapSolarSystemJump&gt;**](MapSolarSystemJump.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getSolarSystems"></a>
# **getSolarSystems**
> List&lt;MapSolarSystem&gt; getSolarSystems(contid, maxresults, solarSystemID, border, constellation, constellationID, corridor, factionID, fringe, hub, international, luminosity, radius, regional, regionID, security, securityClass, solarSystemName, sunTypeID, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin)

Get solar systems



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String solarSystemID = "{ any: true }"; // String | Solar system ID selector
String border = "{ any: true }"; // String | Border flag selector
String constellation = "{ any: true }"; // String | Constellation selector
String constellationID = "{ any: true }"; // String | Constellation ID selector
String corridor = "{ any: true }"; // String | Corridor flag selector
String factionID = "{ any: true }"; // String | Faction ID selector
String fringe = "{ any: true }"; // String | Fringe flag selector
String hub = "{ any: true }"; // String | Hub flag selector
String international = "{ any: true }"; // String | International flag selector
String luminosity = "{ any: true }"; // String | Luminosity selector
String radius = "{ any: true }"; // String | Radius selector
String regional = "{ any: true }"; // String | Regional flag selector
String regionID = "{ any: true }"; // String | Region ID selector
String security = "{ any: true }"; // String | Security selector
String securityClass = "{ any: true }"; // String | Security class selector
String solarSystemName = "{ any: true }"; // String | Solar system name selector
String sunTypeID = "{ any: true }"; // String | Sun type ID selector
String x = "{ any: true }"; // String | X position selector
String xMax = "{ any: true }"; // String | Max X extent selector
String xMin = "{ any: true }"; // String | Min X extent selector
String y = "{ any: true }"; // String | Y position selector
String yMax = "{ any: true }"; // String | Max Y extent selector
String yMin = "{ any: true }"; // String | Min Y extent selector
String z = "{ any: true }"; // String | Z position selector
String zMax = "{ any: true }"; // String | Max Z extent selector
String zMin = "{ any: true }"; // String | Min Z extent selector
try {
    List<MapSolarSystem> result = apiInstance.getSolarSystems(contid, maxresults, solarSystemID, border, constellation, constellationID, corridor, factionID, fringe, hub, international, luminosity, radius, regional, regionID, security, securityClass, solarSystemName, sunTypeID, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getSolarSystems");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **solarSystemID** | **String**| Solar system ID selector | [optional] [default to { any: true }]
 **border** | **String**| Border flag selector | [optional] [default to { any: true }]
 **constellation** | **String**| Constellation selector | [optional] [default to { any: true }]
 **constellationID** | **String**| Constellation ID selector | [optional] [default to { any: true }]
 **corridor** | **String**| Corridor flag selector | [optional] [default to { any: true }]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]
 **fringe** | **String**| Fringe flag selector | [optional] [default to { any: true }]
 **hub** | **String**| Hub flag selector | [optional] [default to { any: true }]
 **international** | **String**| International flag selector | [optional] [default to { any: true }]
 **luminosity** | **String**| Luminosity selector | [optional] [default to { any: true }]
 **radius** | **String**| Radius selector | [optional] [default to { any: true }]
 **regional** | **String**| Regional flag selector | [optional] [default to { any: true }]
 **regionID** | **String**| Region ID selector | [optional] [default to { any: true }]
 **security** | **String**| Security selector | [optional] [default to { any: true }]
 **securityClass** | **String**| Security class selector | [optional] [default to { any: true }]
 **solarSystemName** | **String**| Solar system name selector | [optional] [default to { any: true }]
 **sunTypeID** | **String**| Sun type ID selector | [optional] [default to { any: true }]
 **x** | **String**| X position selector | [optional] [default to { any: true }]
 **xMax** | **String**| Max X extent selector | [optional] [default to { any: true }]
 **xMin** | **String**| Min X extent selector | [optional] [default to { any: true }]
 **y** | **String**| Y position selector | [optional] [default to { any: true }]
 **yMax** | **String**| Max Y extent selector | [optional] [default to { any: true }]
 **yMin** | **String**| Min Y extent selector | [optional] [default to { any: true }]
 **z** | **String**| Z position selector | [optional] [default to { any: true }]
 **zMax** | **String**| Max Z extent selector | [optional] [default to { any: true }]
 **zMin** | **String**| Min Z extent selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapSolarSystem&gt;**](MapSolarSystem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getUniverses"></a>
# **getUniverses**
> List&lt;MapUniverse&gt; getUniverses(contid, maxresults, universeID, radius, universeName, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin)

Get universes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.MapApi;


MapApi apiInstance = new MapApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String universeID = "{ any: true }"; // String | Universe ID selector
String radius = "{ any: true }"; // String | Radius selector
String universeName = "{ any: true }"; // String | Universe name selector
String x = "{ any: true }"; // String | X position selector
String xMax = "{ any: true }"; // String | Max X extent selector
String xMin = "{ any: true }"; // String | Min X extent selector
String y = "{ any: true }"; // String | Y position selector
String yMax = "{ any: true }"; // String | Max Y extent selector
String yMin = "{ any: true }"; // String | Min Y extent selector
String z = "{ any: true }"; // String | Z position selector
String zMax = "{ any: true }"; // String | Max Z extent selector
String zMin = "{ any: true }"; // String | Min Z extent selector
try {
    List<MapUniverse> result = apiInstance.getUniverses(contid, maxresults, universeID, radius, universeName, x, xMax, xMin, y, yMax, yMin, z, zMax, zMin);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MapApi#getUniverses");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **universeID** | **String**| Universe ID selector | [optional] [default to { any: true }]
 **radius** | **String**| Radius selector | [optional] [default to { any: true }]
 **universeName** | **String**| Universe name selector | [optional] [default to { any: true }]
 **x** | **String**| X position selector | [optional] [default to { any: true }]
 **xMax** | **String**| Max X extent selector | [optional] [default to { any: true }]
 **xMin** | **String**| Min X extent selector | [optional] [default to { any: true }]
 **y** | **String**| Y position selector | [optional] [default to { any: true }]
 **yMax** | **String**| Max Y extent selector | [optional] [default to { any: true }]
 **yMin** | **String**| Min Y extent selector | [optional] [default to { any: true }]
 **z** | **String**| Z position selector | [optional] [default to { any: true }]
 **zMax** | **String**| Max Z extent selector | [optional] [default to { any: true }]
 **zMin** | **String**| Min Z extent selector | [optional] [default to { any: true }]

### Return type

[**List&lt;MapUniverse&gt;**](MapUniverse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

