# InventoryApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20190625/api/ws/v20190625*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCategories**](InventoryApi.md#getCategories) | **GET** /inv/category | Get categories
[**getContrabandTypes**](InventoryApi.md#getContrabandTypes) | **GET** /inv/contraband_type | Get contraband types
[**getControlTowerResourcePurposes**](InventoryApi.md#getControlTowerResourcePurposes) | **GET** /inv/control_tower_resource_purpose | Get control tower resource purposes
[**getControlTowerResources**](InventoryApi.md#getControlTowerResources) | **GET** /inv/control_tower_resource | Get control tower resources
[**getFlags**](InventoryApi.md#getFlags) | **GET** /inv/flag | Get flags
[**getGroups**](InventoryApi.md#getGroups) | **GET** /inv/group | Get groups
[**getItems**](InventoryApi.md#getItems) | **GET** /inv/item | Get items
[**getMetaGroups**](InventoryApi.md#getMetaGroups) | **GET** /inv/meta_group | Get meta groups
[**getMetaTypes**](InventoryApi.md#getMetaTypes) | **GET** /inv/meta_type | Get meta types
[**getNames**](InventoryApi.md#getNames) | **GET** /inv/name | Get names
[**getPositions**](InventoryApi.md#getPositions) | **GET** /inv/position | Get positions
[**getTraits**](InventoryApi.md#getTraits) | **GET** /inv/trait | Get traits
[**getTypeMaterials**](InventoryApi.md#getTypeMaterials) | **GET** /inv/type_material | Get type materials
[**getTypeReactions**](InventoryApi.md#getTypeReactions) | **GET** /inv/type_reaction | Get type reactions
[**getTypes**](InventoryApi.md#getTypes) | **GET** /inv/type | Get types
[**getUniqueNames**](InventoryApi.md#getUniqueNames) | **GET** /inv/unique_name | Get unique names
[**getVolumes**](InventoryApi.md#getVolumes) | **GET** /inv/volume | Get type volumes


<a name="getCategories"></a>
# **getCategories**
> List&lt;InvCategory&gt; getCategories(contid, maxresults, categoryID, categoryName, iconID, published)

Get categories



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String categoryID = "{ any: true }"; // String | Category ID selector
String categoryName = "{ any: true }"; // String | Category name selector
String iconID = "{ any: true }"; // String | Icon ID selector
String published = "{ any: true }"; // String | Published flag selector
try {
    List<InvCategory> result = apiInstance.getCategories(contid, maxresults, categoryID, categoryName, iconID, published);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **categoryID** | **String**| Category ID selector | [optional] [default to { any: true }]
 **categoryName** | **String**| Category name selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **published** | **String**| Published flag selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvCategory&gt;**](InvCategory.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getContrabandTypes"></a>
# **getContrabandTypes**
> List&lt;InvContrabandType&gt; getContrabandTypes(contid, maxresults, factionID, typeID, attackMinSec, confiscateMinSec, fineByValue, standingLoss)

Get contraband types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String factionID = "{ any: true }"; // String | Faction ID selector
String typeID = "{ any: true }"; // String | Type ID selector
String attackMinSec = "{ any: true }"; // String | Attack minimum security level selector
String confiscateMinSec = "{ any: true }"; // String | Confiscation minimum security level selector
String fineByValue = "{ any: true }"; // String | Fine by value selector
String standingLoss = "{ any: true }"; // String | Standing loss selector
try {
    List<InvContrabandType> result = apiInstance.getContrabandTypes(contid, maxresults, factionID, typeID, attackMinSec, confiscateMinSec, fineByValue, standingLoss);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getContrabandTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **attackMinSec** | **String**| Attack minimum security level selector | [optional] [default to { any: true }]
 **confiscateMinSec** | **String**| Confiscation minimum security level selector | [optional] [default to { any: true }]
 **fineByValue** | **String**| Fine by value selector | [optional] [default to { any: true }]
 **standingLoss** | **String**| Standing loss selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvContrabandType&gt;**](InvContrabandType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getControlTowerResourcePurposes"></a>
# **getControlTowerResourcePurposes**
> List&lt;InvControlTowerResourcePurpose&gt; getControlTowerResourcePurposes(contid, maxresults, purpose, purposeText)

Get control tower resource purposes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String purpose = "{ any: true }"; // String | Purpose selector
String purposeText = "{ any: true }"; // String | Purpose text selector
try {
    List<InvControlTowerResourcePurpose> result = apiInstance.getControlTowerResourcePurposes(contid, maxresults, purpose, purposeText);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getControlTowerResourcePurposes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **purpose** | **String**| Purpose selector | [optional] [default to { any: true }]
 **purposeText** | **String**| Purpose text selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvControlTowerResourcePurpose&gt;**](InvControlTowerResourcePurpose.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getControlTowerResources"></a>
# **getControlTowerResources**
> List&lt;InvControlTowerResource&gt; getControlTowerResources(contid, maxresults, controlTowerTypeID, resourceTypeID, factionID, minSecurityLevel, purpose, quantity)

Get control tower resources



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String controlTowerTypeID = "{ any: true }"; // String | Control tower type ID selector
String resourceTypeID = "{ any: true }"; // String | Resource type ID selector
String factionID = "{ any: true }"; // String | Faction ID selector
String minSecurityLevel = "{ any: true }"; // String | Minimum security level selector
String purpose = "{ any: true }"; // String | Purpose selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<InvControlTowerResource> result = apiInstance.getControlTowerResources(contid, maxresults, controlTowerTypeID, resourceTypeID, factionID, minSecurityLevel, purpose, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getControlTowerResources");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **controlTowerTypeID** | **String**| Control tower type ID selector | [optional] [default to { any: true }]
 **resourceTypeID** | **String**| Resource type ID selector | [optional] [default to { any: true }]
 **factionID** | **String**| Faction ID selector | [optional] [default to { any: true }]
 **minSecurityLevel** | **String**| Minimum security level selector | [optional] [default to { any: true }]
 **purpose** | **String**| Purpose selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvControlTowerResource&gt;**](InvControlTowerResource.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getFlags"></a>
# **getFlags**
> List&lt;InvFlag&gt; getFlags(contid, maxresults, flagID, flagName, flagText, orderID)

Get flags



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String flagID = "{ any: true }"; // String | Flag ID selector
String flagName = "{ any: true }"; // String | Flag name selector
String flagText = "{ any: true }"; // String | Flag text selector
String orderID = "{ any: true }"; // String | Order ID selector
try {
    List<InvFlag> result = apiInstance.getFlags(contid, maxresults, flagID, flagName, flagText, orderID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getFlags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **flagID** | **String**| Flag ID selector | [optional] [default to { any: true }]
 **flagName** | **String**| Flag name selector | [optional] [default to { any: true }]
 **flagText** | **String**| Flag text selector | [optional] [default to { any: true }]
 **orderID** | **String**| Order ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvFlag&gt;**](InvFlag.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getGroups"></a>
# **getGroups**
> List&lt;InvGroup&gt; getGroups(contid, maxresults, groupID, anchorable, anchored, categoryID, fittableNonSingleton, groupName, iconID, published, useBasePrice)

Get groups



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String groupID = "{ any: true }"; // String | Group ID selector
String anchorable = "{ any: true }"; // String | Anchorable flag selector
String anchored = "{ any: true }"; // String | Anchored flag selector
String categoryID = "{ any: true }"; // String | Category ID selector
String fittableNonSingleton = "{ any: true }"; // String | Fittable non-singleton flag selector
String groupName = "{ any: true }"; // String | Group name selector
String iconID = "{ any: true }"; // String | Icon ID selector
String published = "{ any: true }"; // String | Published flag selector
String useBasePrice = "{ any: true }"; // String | Use base price selector
try {
    List<InvGroup> result = apiInstance.getGroups(contid, maxresults, groupID, anchorable, anchored, categoryID, fittableNonSingleton, groupName, iconID, published, useBasePrice);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getGroups");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **groupID** | **String**| Group ID selector | [optional] [default to { any: true }]
 **anchorable** | **String**| Anchorable flag selector | [optional] [default to { any: true }]
 **anchored** | **String**| Anchored flag selector | [optional] [default to { any: true }]
 **categoryID** | **String**| Category ID selector | [optional] [default to { any: true }]
 **fittableNonSingleton** | **String**| Fittable non-singleton flag selector | [optional] [default to { any: true }]
 **groupName** | **String**| Group name selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **published** | **String**| Published flag selector | [optional] [default to { any: true }]
 **useBasePrice** | **String**| Use base price selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvGroup&gt;**](InvGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getItems"></a>
# **getItems**
> List&lt;InvItem&gt; getItems(contid, maxresults, itemID, flagID, locationID, ownerID, quantity, typeID)

Get items



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String itemID = "{ any: true }"; // String | Item ID selector
String flagID = "{ any: true }"; // String | Flag ID selector
String locationID = "{ any: true }"; // String | Location ID selector
String ownerID = "{ any: true }"; // String | Owner ID selector
String quantity = "{ any: true }"; // String | Quantity selector
String typeID = "{ any: true }"; // String | Type ID selector
try {
    List<InvItem> result = apiInstance.getItems(contid, maxresults, itemID, flagID, locationID, ownerID, quantity, typeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getItems");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **itemID** | **String**| Item ID selector | [optional] [default to { any: true }]
 **flagID** | **String**| Flag ID selector | [optional] [default to { any: true }]
 **locationID** | **String**| Location ID selector | [optional] [default to { any: true }]
 **ownerID** | **String**| Owner ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvItem&gt;**](InvItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getMetaGroups"></a>
# **getMetaGroups**
> List&lt;InvMetaGroup&gt; getMetaGroups(contid, maxresults, metaGroupID, description, iconID, metaGroupName)

Get meta groups



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String metaGroupID = "{ any: true }"; // String | Meta group ID selector
String description = "{ any: true }"; // String | Description text selector
String iconID = "{ any: true }"; // String | Icon ID selector
String metaGroupName = "{ any: true }"; // String | Meta group name selector
try {
    List<InvMetaGroup> result = apiInstance.getMetaGroups(contid, maxresults, metaGroupID, description, iconID, metaGroupName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getMetaGroups");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **metaGroupID** | **String**| Meta group ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **metaGroupName** | **String**| Meta group name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvMetaGroup&gt;**](InvMetaGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getMetaTypes"></a>
# **getMetaTypes**
> List&lt;InvMetaType&gt; getMetaTypes(contid, maxresults, typeID, metaGroupID, parentTypeID)

Get meta types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String metaGroupID = "{ any: true }"; // String | Meta group ID selector
String parentTypeID = "{ any: true }"; // String | Parent type ID selector
try {
    List<InvMetaType> result = apiInstance.getMetaTypes(contid, maxresults, typeID, metaGroupID, parentTypeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getMetaTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **metaGroupID** | **String**| Meta group ID selector | [optional] [default to { any: true }]
 **parentTypeID** | **String**| Parent type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvMetaType&gt;**](InvMetaType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getNames"></a>
# **getNames**
> List&lt;InvName&gt; getNames(contid, maxresults, itemID, itemName)

Get names



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String itemID = "{ any: true }"; // String | Item ID selector
String itemName = "{ any: true }"; // String | Item name selector
try {
    List<InvName> result = apiInstance.getNames(contid, maxresults, itemID, itemName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getNames");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **itemID** | **String**| Item ID selector | [optional] [default to { any: true }]
 **itemName** | **String**| Item name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvName&gt;**](InvName.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getPositions"></a>
# **getPositions**
> List&lt;InvPosition&gt; getPositions(contid, maxresults, itemID, pitch, roll, x, y, yaw, z)

Get positions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String itemID = "{ any: true }"; // String | Item ID selector
String pitch = "{ any: true }"; // String | Pitch selector
String roll = "{ any: true }"; // String | Roll selector
String x = "{ any: true }"; // String | X selector
String y = "{ any: true }"; // String | Y selector
String yaw = "{ any: true }"; // String | Yaw selector
String z = "{ any: true }"; // String | Z selector
try {
    List<InvPosition> result = apiInstance.getPositions(contid, maxresults, itemID, pitch, roll, x, y, yaw, z);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getPositions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **itemID** | **String**| Item ID selector | [optional] [default to { any: true }]
 **pitch** | **String**| Pitch selector | [optional] [default to { any: true }]
 **roll** | **String**| Roll selector | [optional] [default to { any: true }]
 **x** | **String**| X selector | [optional] [default to { any: true }]
 **y** | **String**| Y selector | [optional] [default to { any: true }]
 **yaw** | **String**| Yaw selector | [optional] [default to { any: true }]
 **z** | **String**| Z selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvPosition&gt;**](InvPosition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTraits"></a>
# **getTraits**
> List&lt;InvTrait&gt; getTraits(contid, maxresults, traitID, typeID, skillID, bonus, bonusText, unitID)

Get traits



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String traitID = "{ any: true }"; // String | Trait ID selector
String typeID = "{ any: true }"; // String | Trait ID selector
String skillID = "{ any: true }"; // String | Skill ID selector
String bonus = "{ any: true }"; // String | Bonus selector
String bonusText = "{ any: true }"; // String | Bonus text selector
String unitID = "{ any: true }"; // String | Unit ID selector
try {
    List<InvTrait> result = apiInstance.getTraits(contid, maxresults, traitID, typeID, skillID, bonus, bonusText, unitID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getTraits");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **traitID** | **String**| Trait ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Trait ID selector | [optional] [default to { any: true }]
 **skillID** | **String**| Skill ID selector | [optional] [default to { any: true }]
 **bonus** | **String**| Bonus selector | [optional] [default to { any: true }]
 **bonusText** | **String**| Bonus text selector | [optional] [default to { any: true }]
 **unitID** | **String**| Unit ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvTrait&gt;**](InvTrait.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTypeMaterials"></a>
# **getTypeMaterials**
> List&lt;InvTypeMaterial&gt; getTypeMaterials(contid, maxresults, typeID, materialTypeID, quantity)

Get type materials



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String materialTypeID = "{ any: true }"; // String | Material type ID selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<InvTypeMaterial> result = apiInstance.getTypeMaterials(contid, maxresults, typeID, materialTypeID, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getTypeMaterials");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **materialTypeID** | **String**| Material type ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvTypeMaterial&gt;**](InvTypeMaterial.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTypeReactions"></a>
# **getTypeReactions**
> List&lt;InvTypeReaction&gt; getTypeReactions(contid, maxresults, reactionTypeID, input, typeID, quantity)

Get type reactions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String reactionTypeID = "{ any: true }"; // String | Reaction type ID selector
String input = "{ any: true }"; // String | Input selector
String typeID = "{ any: true }"; // String | Type ID selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<InvTypeReaction> result = apiInstance.getTypeReactions(contid, maxresults, reactionTypeID, input, typeID, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getTypeReactions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **reactionTypeID** | **String**| Reaction type ID selector | [optional] [default to { any: true }]
 **input** | **String**| Input selector | [optional] [default to { any: true }]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvTypeReaction&gt;**](InvTypeReaction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTypes"></a>
# **getTypes**
> List&lt;InvType&gt; getTypes(contid, maxresults, typeID, basePrice, capacity, chanceOfDuplicating, description, graphicID, groupID, iconID, marketGroupID, mass, portionSize, published, raceID, soundID, typeName, volume)

Get types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String basePrice = "{ any: true }"; // String | Base price selector
String capacity = "{ any: true }"; // String | Capacity selector
String chanceOfDuplicating = "{ any: true }"; // String | Chance of duplicating selector
String description = "{ any: true }"; // String | Description text selector
String graphicID = "{ any: true }"; // String | Graphic ID selector
String groupID = "{ any: true }"; // String | Group ID selector
String iconID = "{ any: true }"; // String | Icon ID selector
String marketGroupID = "{ any: true }"; // String | Market group ID selector
String mass = "{ any: true }"; // String | Mass selector
String portionSize = "{ any: true }"; // String | Portion size selector
String published = "{ any: true }"; // String | Published flag selector
String raceID = "{ any: true }"; // String | Race ID selector
String soundID = "{ any: true }"; // String | Sound ID selector
String typeName = "{ any: true }"; // String | Type name selector
String volume = "{ any: true }"; // String | Volume selector
try {
    List<InvType> result = apiInstance.getTypes(contid, maxresults, typeID, basePrice, capacity, chanceOfDuplicating, description, graphicID, groupID, iconID, marketGroupID, mass, portionSize, published, raceID, soundID, typeName, volume);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **basePrice** | **String**| Base price selector | [optional] [default to { any: true }]
 **capacity** | **String**| Capacity selector | [optional] [default to { any: true }]
 **chanceOfDuplicating** | **String**| Chance of duplicating selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **graphicID** | **String**| Graphic ID selector | [optional] [default to { any: true }]
 **groupID** | **String**| Group ID selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **marketGroupID** | **String**| Market group ID selector | [optional] [default to { any: true }]
 **mass** | **String**| Mass selector | [optional] [default to { any: true }]
 **portionSize** | **String**| Portion size selector | [optional] [default to { any: true }]
 **published** | **String**| Published flag selector | [optional] [default to { any: true }]
 **raceID** | **String**| Race ID selector | [optional] [default to { any: true }]
 **soundID** | **String**| Sound ID selector | [optional] [default to { any: true }]
 **typeName** | **String**| Type name selector | [optional] [default to { any: true }]
 **volume** | **String**| Volume selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvType&gt;**](InvType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getUniqueNames"></a>
# **getUniqueNames**
> List&lt;InvUniqueName&gt; getUniqueNames(contid, maxresults, itemID, groupID, itemName)

Get unique names



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String itemID = "{ any: true }"; // String | Item ID selector
String groupID = "{ any: true }"; // String | Group ID selector
String itemName = "{ any: true }"; // String | Item name selector
try {
    List<InvUniqueName> result = apiInstance.getUniqueNames(contid, maxresults, itemID, groupID, itemName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getUniqueNames");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **itemID** | **String**| Item ID selector | [optional] [default to { any: true }]
 **groupID** | **String**| Group ID selector | [optional] [default to { any: true }]
 **itemName** | **String**| Item name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvUniqueName&gt;**](InvUniqueName.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getVolumes"></a>
# **getVolumes**
> List&lt;InvVolume&gt; getVolumes(contid, maxresults, typeID, volume)

Get type volumes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.InventoryApi;


InventoryApi apiInstance = new InventoryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String volume = "{ any: true }"; // String | Volume selector
try {
    List<InvVolume> result = apiInstance.getVolumes(contid, maxresults, typeID, volume);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryApi#getVolumes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **volume** | **String**| Volume selector | [optional] [default to { any: true }]

### Return type

[**List&lt;InvVolume&gt;**](InvVolume.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

