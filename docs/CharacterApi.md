# CharacterApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180214/api/ws/v20180214*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAncestries**](CharacterApi.md#getAncestries) | **GET** /chr/ancestry | Get ancestries
[**getAttributes**](CharacterApi.md#getAttributes) | **GET** /chr/attribute | Get attributes
[**getBloodlines**](CharacterApi.md#getBloodlines) | **GET** /chr/bloodline | Get bloodlines
[**getFactions**](CharacterApi.md#getFactions) | **GET** /chr/faction | Get factions
[**getRaces**](CharacterApi.md#getRaces) | **GET** /chr/race | Get races


<a name="getAncestries"></a>
# **getAncestries**
> List&lt;ChrAncestry&gt; getAncestries(contid, maxresults, ancestryID, ancestryName, bloodlineID, charisma, description, iconID, intelligence, memory, perception, shortDescription, willpower)

Get ancestries



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CharacterApi;


CharacterApi apiInstance = new CharacterApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String ancestryID = "{ any: true }"; // String | Ancestry ID selector
String ancestryName = "{ any: true }"; // String | Ancestry name selector
String bloodlineID = "{ any: true }"; // String | Bloodline ID selector
String charisma = "{ any: true }"; // String | Charisma value selector
String description = "{ any: true }"; // String | Description text selector
String iconID = "{ any: true }"; // String | Icon ID selector
String intelligence = "{ any: true }"; // String | Intelligence value selector
String memory = "{ any: true }"; // String | Memory value selector
String perception = "{ any: true }"; // String | Perception value selector
String shortDescription = "{ any: true }"; // String | Short description text selector
String willpower = "{ any: true }"; // String | Willpower value selector
try {
    List<ChrAncestry> result = apiInstance.getAncestries(contid, maxresults, ancestryID, ancestryName, bloodlineID, charisma, description, iconID, intelligence, memory, perception, shortDescription, willpower);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CharacterApi#getAncestries");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **ancestryID** | **String**| Ancestry ID selector | [optional] [default to { any: true }]
 **ancestryName** | **String**| Ancestry name selector | [optional] [default to { any: true }]
 **bloodlineID** | **String**| Bloodline ID selector | [optional] [default to { any: true }]
 **charisma** | **String**| Charisma value selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **intelligence** | **String**| Intelligence value selector | [optional] [default to { any: true }]
 **memory** | **String**| Memory value selector | [optional] [default to { any: true }]
 **perception** | **String**| Perception value selector | [optional] [default to { any: true }]
 **shortDescription** | **String**| Short description text selector | [optional] [default to { any: true }]
 **willpower** | **String**| Willpower value selector | [optional] [default to { any: true }]

### Return type

[**List&lt;ChrAncestry&gt;**](ChrAncestry.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getAttributes"></a>
# **getAttributes**
> List&lt;ChrAttribute&gt; getAttributes(contid, maxresults, attributeID, attributeName, description, iconID, notes, shortDescription)

Get attributes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CharacterApi;


CharacterApi apiInstance = new CharacterApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String attributeID = "{ any: true }"; // String | Attribute ID selector
String attributeName = "{ any: true }"; // String | Attribute name selector
String description = "{ any: true }"; // String | Description text selector
String iconID = "{ any: true }"; // String | Icon ID selector
String notes = "{ any: true }"; // String | Notes text selector
String shortDescription = "{ any: true }"; // String | Short description text selector
try {
    List<ChrAttribute> result = apiInstance.getAttributes(contid, maxresults, attributeID, attributeName, description, iconID, notes, shortDescription);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CharacterApi#getAttributes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **attributeID** | **String**| Attribute ID selector | [optional] [default to { any: true }]
 **attributeName** | **String**| Attribute name selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **notes** | **String**| Notes text selector | [optional] [default to { any: true }]
 **shortDescription** | **String**| Short description text selector | [optional] [default to { any: true }]

### Return type

[**List&lt;ChrAttribute&gt;**](ChrAttribute.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getBloodlines"></a>
# **getBloodlines**
> List&lt;ChrBloodline&gt; getBloodlines(contid, maxresults, bloodlineID, bloodlineName, charisma, corporationID, description, femaleDescription, iconID, intelligence, maleDescription, memory, perception, raceID, shipTypeID, shortDescription, shortFemaleDescription, shortMaleDescription, willpower)

Get bloodlines



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CharacterApi;


CharacterApi apiInstance = new CharacterApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String bloodlineID = "{ any: true }"; // String | Bloodline ID selector
String bloodlineName = "{ any: true }"; // String | Bloodline name selector
String charisma = "{ any: true }"; // String | Charisma vlaue selector
String corporationID = "{ any: true }"; // String | Corporation ID selector
String description = "{ any: true }"; // String | Description text selector
String femaleDescription = "{ any: true }"; // String | Female description text selector
String iconID = "{ any: true }"; // String | Icon ID selector
String intelligence = "{ any: true }"; // String | Intelligence value selector
String maleDescription = "{ any: true }"; // String | Male description text selector
String memory = "{ any: true }"; // String | Memory value selector
String perception = "{ any: true }"; // String | Perception value selector
String raceID = "{ any: true }"; // String | Race ID selector
String shipTypeID = "{ any: true }"; // String | Ship type ID selector
String shortDescription = "{ any: true }"; // String | Short description text selector
String shortFemaleDescription = "{ any: true }"; // String | Short female description text selector
String shortMaleDescription = "{ any: true }"; // String | Short male description text selector
String willpower = "{ any: true }"; // String | Willpower value selector
try {
    List<ChrBloodline> result = apiInstance.getBloodlines(contid, maxresults, bloodlineID, bloodlineName, charisma, corporationID, description, femaleDescription, iconID, intelligence, maleDescription, memory, perception, raceID, shipTypeID, shortDescription, shortFemaleDescription, shortMaleDescription, willpower);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CharacterApi#getBloodlines");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **bloodlineID** | **String**| Bloodline ID selector | [optional] [default to { any: true }]
 **bloodlineName** | **String**| Bloodline name selector | [optional] [default to { any: true }]
 **charisma** | **String**| Charisma vlaue selector | [optional] [default to { any: true }]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **femaleDescription** | **String**| Female description text selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **intelligence** | **String**| Intelligence value selector | [optional] [default to { any: true }]
 **maleDescription** | **String**| Male description text selector | [optional] [default to { any: true }]
 **memory** | **String**| Memory value selector | [optional] [default to { any: true }]
 **perception** | **String**| Perception value selector | [optional] [default to { any: true }]
 **raceID** | **String**| Race ID selector | [optional] [default to { any: true }]
 **shipTypeID** | **String**| Ship type ID selector | [optional] [default to { any: true }]
 **shortDescription** | **String**| Short description text selector | [optional] [default to { any: true }]
 **shortFemaleDescription** | **String**| Short female description text selector | [optional] [default to { any: true }]
 **shortMaleDescription** | **String**| Short male description text selector | [optional] [default to { any: true }]
 **willpower** | **String**| Willpower value selector | [optional] [default to { any: true }]

### Return type

[**List&lt;ChrBloodline&gt;**](ChrBloodline.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getFactions"></a>
# **getFactions**
> List&lt;ChrFaction&gt; getFactions(contid, maxresults, factionID, corporationID, description, factionName, iconID, militiaCorporationID, raceIDs, sizeFactor, solarSystemID, stationCount, stationSystemCount)

Get factions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CharacterApi;


CharacterApi apiInstance = new CharacterApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String factionID = "{ any: true }"; // String | Agent ID selector
String corporationID = "{ any: true }"; // String | Agent ID selector
String description = "{ any: true }"; // String | Agent ID selector
String factionName = "{ any: true }"; // String | Agent ID selector
String iconID = "{ any: true }"; // String | Agent ID selector
String militiaCorporationID = "{ any: true }"; // String | Agent ID selector
String raceIDs = "{ any: true }"; // String | Agent ID selector
String sizeFactor = "{ any: true }"; // String | Agent ID selector
String solarSystemID = "{ any: true }"; // String | Agent ID selector
String stationCount = "{ any: true }"; // String | Agent ID selector
String stationSystemCount = "{ any: true }"; // String | Agent ID selector
try {
    List<ChrFaction> result = apiInstance.getFactions(contid, maxresults, factionID, corporationID, description, factionName, iconID, militiaCorporationID, raceIDs, sizeFactor, solarSystemID, stationCount, stationSystemCount);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CharacterApi#getFactions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **factionID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **corporationID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **description** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **factionName** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **iconID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **militiaCorporationID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **raceIDs** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **sizeFactor** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **solarSystemID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **stationCount** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **stationSystemCount** | **String**| Agent ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;ChrFaction&gt;**](ChrFaction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getRaces"></a>
# **getRaces**
> List&lt;ChrRace&gt; getRaces(contid, maxresults, raceID, description, iconID, raceName, shortDescription)

Get races



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CharacterApi;


CharacterApi apiInstance = new CharacterApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String raceID = "{ any: true }"; // String | Race ID selector
String description = "{ any: true }"; // String | Description text selector
String iconID = "{ any: true }"; // String | Icon ID selector
String raceName = "{ any: true }"; // String | Race name selector
String shortDescription = "{ any: true }"; // String | Short description text selector
try {
    List<ChrRace> result = apiInstance.getRaces(contid, maxresults, raceID, description, iconID, raceName, shortDescription);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CharacterApi#getRaces");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **raceID** | **String**| Race ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **raceName** | **String**| Race name selector | [optional] [default to { any: true }]
 **shortDescription** | **String**| Short description text selector | [optional] [default to { any: true }]

### Return type

[**List&lt;ChrRace&gt;**](ChrRace.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

