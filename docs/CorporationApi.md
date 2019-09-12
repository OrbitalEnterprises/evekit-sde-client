# CorporationApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20190625/api/ws/v20190625*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCorpActivities**](CorporationApi.md#getCorpActivities) | **GET** /crp/activity | Get corporation activities
[**getNpcCorporationDivisions**](CorporationApi.md#getNpcCorporationDivisions) | **GET** /crp/npc_corp_division | Get NPC corporation divisions
[**getNpcCorporationResearchFields**](CorporationApi.md#getNpcCorporationResearchFields) | **GET** /crp/npc_corp_research_field | Get NPC corporation research fields
[**getNpcCorporationTrades**](CorporationApi.md#getNpcCorporationTrades) | **GET** /crp/npc_corp_trade | Get NPC corporation trades
[**getNpcCorporations**](CorporationApi.md#getNpcCorporations) | **GET** /crp/npc_corp | Get NPC corporations
[**getNpcDivisions**](CorporationApi.md#getNpcDivisions) | **GET** /crp/npc_division | Get NPC divisions


<a name="getCorpActivities"></a>
# **getCorpActivities**
> List&lt;CrpActivity&gt; getCorpActivities(contid, maxresults, activityID, activityName, description)

Get corporation activities



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CorporationApi;


CorporationApi apiInstance = new CorporationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String activityID = "{ any: true }"; // String | Activity ID selector
String activityName = "{ any: true }"; // String | Activity name selector
String description = "{ any: true }"; // String | Description text selector
try {
    List<CrpActivity> result = apiInstance.getCorpActivities(contid, maxresults, activityID, activityName, description);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CorporationApi#getCorpActivities");
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

### Return type

[**List&lt;CrpActivity&gt;**](CrpActivity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getNpcCorporationDivisions"></a>
# **getNpcCorporationDivisions**
> List&lt;CrpNpcCorporationDivision&gt; getNpcCorporationDivisions(contid, maxresults, corporationID, divisionID, size)

Get NPC corporation divisions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CorporationApi;


CorporationApi apiInstance = new CorporationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String corporationID = "{ any: true }"; // String | Corporation ID selector
String divisionID = "{ any: true }"; // String | Division ID selector
String size = "{ any: true }"; // String | Size selector
try {
    List<CrpNpcCorporationDivision> result = apiInstance.getNpcCorporationDivisions(contid, maxresults, corporationID, divisionID, size);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CorporationApi#getNpcCorporationDivisions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]
 **divisionID** | **String**| Division ID selector | [optional] [default to { any: true }]
 **size** | **String**| Size selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrpNpcCorporationDivision&gt;**](CrpNpcCorporationDivision.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getNpcCorporationResearchFields"></a>
# **getNpcCorporationResearchFields**
> List&lt;CrpNpcCorporationResearchField&gt; getNpcCorporationResearchFields(contid, maxresults, skillID, corporationID)

Get NPC corporation research fields



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CorporationApi;


CorporationApi apiInstance = new CorporationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String skillID = "{ any: true }"; // String | Skill ID selector
String corporationID = "{ any: true }"; // String | Corporation ID selector
try {
    List<CrpNpcCorporationResearchField> result = apiInstance.getNpcCorporationResearchFields(contid, maxresults, skillID, corporationID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CorporationApi#getNpcCorporationResearchFields");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **skillID** | **String**| Skill ID selector | [optional] [default to { any: true }]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrpNpcCorporationResearchField&gt;**](CrpNpcCorporationResearchField.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getNpcCorporationTrades"></a>
# **getNpcCorporationTrades**
> List&lt;CrpNpcCorporationTrade&gt; getNpcCorporationTrades(contid, maxresults, corporationID, typeID)

Get NPC corporation trades



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CorporationApi;


CorporationApi apiInstance = new CorporationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String corporationID = "{ any: true }"; // String | Corporation ID selector
String typeID = "{ any: true }"; // String | Type ID selector
try {
    List<CrpNpcCorporationTrade> result = apiInstance.getNpcCorporationTrades(contid, maxresults, corporationID, typeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CorporationApi#getNpcCorporationTrades");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrpNpcCorporationTrade&gt;**](CrpNpcCorporationTrade.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getNpcCorporations"></a>
# **getNpcCorporations**
> List&lt;CrpNpcCorporation&gt; getNpcCorporations(contid, maxresults, corporationID, border, corridor, description, enemyID, extent, factionID, friendID, fringe, hub, iconID, initialPrice, investorID1, investorID2, investorID3, investorID4, investorShares1, investorShares2, investorShares3, investorShares4, minSecurity, publicShares, scattered, size, sizeFactor, solarSystemID, stationCount, stationSystemCount)

Get NPC corporations



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CorporationApi;


CorporationApi apiInstance = new CorporationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String corporationID = "{ any: true }"; // String | Corporation ID selector
String border = "{ any: true }"; // String | Border attribute selector
String corridor = "{ any: true }"; // String | Corridor attribute selector
String description = "{ any: true }"; // String | Description text selector
String enemyID = "{ any: true }"; // String | Enemy ID selector
String extent = "{ any: true }"; // String | Extent selector
String factionID = "{ any: true }"; // String | Faction ID selector
String friendID = "{ any: true }"; // String | Friend ID selector
String fringe = "{ any: true }"; // String | Fringe attribute selector
String hub = "{ any: true }"; // String | Hub attribute selector
String iconID = "{ any: true }"; // String | Icon ID selector
String initialPrice = "{ any: true }"; // String | Initial price selector
String investorID1 = "{ any: true }"; // String | First investor ID selector
String investorID2 = "{ any: true }"; // String | Second investor ID selector
String investorID3 = "{ any: true }"; // String | Third investor ID selector
String investorID4 = "{ any: true }"; // String | Fourth investor ID selector
String investorShares1 = "{ any: true }"; // String | First investor shares selector
String investorShares2 = "{ any: true }"; // String | Second investor shares selector
String investorShares3 = "{ any: true }"; // String | Third investor shares selector
String investorShares4 = "{ any: true }"; // String | Fourth investor shares selector
String minSecurity = "{ any: true }"; // String | Minimum security selector
String publicShares = "{ any: true }"; // String | Public shares selector
String scattered = "{ any: true }"; // String | Scattered attribute selector
String size = "{ any: true }"; // String | Size selector
String sizeFactor = "{ any: true }"; // String | Size factor selector
String solarSystemID = "{ any: true }"; // String | Solar system IDselector
String stationCount = "{ any: true }"; // String | Station count selector
String stationSystemCount = "{ any: true }"; // String | Station system count selector
try {
    List<CrpNpcCorporation> result = apiInstance.getNpcCorporations(contid, maxresults, corporationID, border, corridor, description, enemyID, extent, factionID, friendID, fringe, hub, iconID, initialPrice, investorID1, investorID2, investorID3, investorID4, investorShares1, investorShares2, investorShares3, investorShares4, minSecurity, publicShares, scattered, size, sizeFactor, solarSystemID, stationCount, stationSystemCount);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CorporationApi#getNpcCorporations");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]
 **border** | **String**| Border attribute selector | [optional] [default to { any: true }]
 **corridor** | **String**| Corridor attribute selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **enemyID** | **String**| Enemy ID selector | [optional] [default to { any: true }]
 **extent** | **String**| Extent selector | [optional] [default to { any: true }]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]
 **friendID** | **String**| Friend ID selector | [optional] [default to { any: true }]
 **fringe** | **String**| Fringe attribute selector | [optional] [default to { any: true }]
 **hub** | **String**| Hub attribute selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **initialPrice** | **String**| Initial price selector | [optional] [default to { any: true }]
 **investorID1** | **String**| First investor ID selector | [optional] [default to { any: true }]
 **investorID2** | **String**| Second investor ID selector | [optional] [default to { any: true }]
 **investorID3** | **String**| Third investor ID selector | [optional] [default to { any: true }]
 **investorID4** | **String**| Fourth investor ID selector | [optional] [default to { any: true }]
 **investorShares1** | **String**| First investor shares selector | [optional] [default to { any: true }]
 **investorShares2** | **String**| Second investor shares selector | [optional] [default to { any: true }]
 **investorShares3** | **String**| Third investor shares selector | [optional] [default to { any: true }]
 **investorShares4** | **String**| Fourth investor shares selector | [optional] [default to { any: true }]
 **minSecurity** | **String**| Minimum security selector | [optional] [default to { any: true }]
 **publicShares** | **String**| Public shares selector | [optional] [default to { any: true }]
 **scattered** | **String**| Scattered attribute selector | [optional] [default to { any: true }]
 **size** | **String**| Size selector | [optional] [default to { any: true }]
 **sizeFactor** | **String**| Size factor selector | [optional] [default to { any: true }]
 **solarSystemID** | **String**| Solar system IDselector | [optional] [default to { any: true }]
 **stationCount** | **String**| Station count selector | [optional] [default to { any: true }]
 **stationSystemCount** | **String**| Station system count selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrpNpcCorporation&gt;**](CrpNpcCorporation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getNpcDivisions"></a>
# **getNpcDivisions**
> List&lt;CrpNpcDivision&gt; getNpcDivisions(contid, maxresults, divisionID, description, divisionName, leaderType)

Get NPC divisions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CorporationApi;


CorporationApi apiInstance = new CorporationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String divisionID = "{ any: true }"; // String | Division ID selector
String description = "{ any: true }"; // String | Description text selector
String divisionName = "{ any: true }"; // String | Division name selector
String leaderType = "{ any: true }"; // String | Leader type selector
try {
    List<CrpNpcDivision> result = apiInstance.getNpcDivisions(contid, maxresults, divisionID, description, divisionName, leaderType);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CorporationApi#getNpcDivisions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **divisionID** | **String**| Division ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **divisionName** | **String**| Division name selector | [optional] [default to { any: true }]
 **leaderType** | **String**| Leader type selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrpNpcDivision&gt;**](CrpNpcDivision.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

