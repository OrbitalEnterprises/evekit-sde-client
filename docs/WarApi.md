# WarApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180827/api/ws/v20180827*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCombatZoneSystems**](WarApi.md#getCombatZoneSystems) | **GET** /war/combat_zone_system | Get combat zone systems
[**getCombatZones**](WarApi.md#getCombatZones) | **GET** /war/combat_zone | Get combat zones


<a name="getCombatZoneSystems"></a>
# **getCombatZoneSystems**
> List&lt;WarCombatZoneSystem&gt; getCombatZoneSystems(contid, maxresults, solarSystemID, combatZoneID)

Get combat zone systems



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.WarApi;


WarApi apiInstance = new WarApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String solarSystemID = "{ any: true }"; // String | Solar system ID selector
String combatZoneID = "{ any: true }"; // String | Combat zone ID selector
try {
    List<WarCombatZoneSystem> result = apiInstance.getCombatZoneSystems(contid, maxresults, solarSystemID, combatZoneID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarApi#getCombatZoneSystems");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **solarSystemID** | **String**| Solar system ID selector | [optional] [default to { any: true }]
 **combatZoneID** | **String**| Combat zone ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;WarCombatZoneSystem&gt;**](WarCombatZoneSystem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getCombatZones"></a>
# **getCombatZones**
> List&lt;WarCombatZone&gt; getCombatZones(contid, maxresults, combatZoneID, centerSystemID, combatZoneName, description, factionID)

Get combat zones



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.WarApi;


WarApi apiInstance = new WarApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String combatZoneID = "{ any: true }"; // String | Combat zone ID selector
String centerSystemID = "{ any: true }"; // String | Center system ID selector
String combatZoneName = "{ any: true }"; // String | Combat zone name selector
String description = "{ any: true }"; // String | Description text selector
String factionID = "{ any: true }"; // String | Faction ID selector
try {
    List<WarCombatZone> result = apiInstance.getCombatZones(contid, maxresults, combatZoneID, centerSystemID, combatZoneName, description, factionID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarApi#getCombatZones");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **combatZoneID** | **String**| Combat zone ID selector | [optional] [default to { any: true }]
 **centerSystemID** | **String**| Center system ID selector | [optional] [default to { any: true }]
 **combatZoneName** | **String**| Combat zone name selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;WarCombatZone&gt;**](WarCombatZone.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

