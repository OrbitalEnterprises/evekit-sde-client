# DogmaApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20190117/api/ws/v20190117*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAttributeCategories**](DogmaApi.md#getAttributeCategories) | **GET** /dgm/attribute_category | Get attribute categories
[**getAttributeTypes**](DogmaApi.md#getAttributeTypes) | **GET** /dgm/attribute_type | Get attribute types
[**getEffects**](DogmaApi.md#getEffects) | **GET** /dgm/effect | Get effects
[**getExpressions**](DogmaApi.md#getExpressions) | **GET** /dgm/expression | Get expressions
[**getTypeAttributes**](DogmaApi.md#getTypeAttributes) | **GET** /dgm/type_attribute | Get type attributes
[**getTypeEffects**](DogmaApi.md#getTypeEffects) | **GET** /dgm/type_effect | Get type effects


<a name="getAttributeCategories"></a>
# **getAttributeCategories**
> List&lt;DgmAttributeCategory&gt; getAttributeCategories(contid, maxresults, categoryID, categoryDescription, categoryName)

Get attribute categories



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.DogmaApi;


DogmaApi apiInstance = new DogmaApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String categoryID = "{ any: true }"; // String | Category ID selector
String categoryDescription = "{ any: true }"; // String | Category description selector
String categoryName = "{ any: true }"; // String | Category name selector
try {
    List<DgmAttributeCategory> result = apiInstance.getAttributeCategories(contid, maxresults, categoryID, categoryDescription, categoryName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DogmaApi#getAttributeCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **categoryID** | **String**| Category ID selector | [optional] [default to { any: true }]
 **categoryDescription** | **String**| Category description selector | [optional] [default to { any: true }]
 **categoryName** | **String**| Category name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;DgmAttributeCategory&gt;**](DgmAttributeCategory.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getAttributeTypes"></a>
# **getAttributeTypes**
> List&lt;DgmAttributeType&gt; getAttributeTypes(contid, maxresults, attributeID, attributeName, categoryID, defaultValue, description, displayName, highIsGood, iconID, published, stackable, unitID)

Get attribute types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.DogmaApi;


DogmaApi apiInstance = new DogmaApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String attributeID = "{ any: true }"; // String | Attribute ID selector
String attributeName = "{ any: true }"; // String | Attribute name selector
String categoryID = "{ any: true }"; // String | Category ID selector
String defaultValue = "{ any: true }"; // String | Default value selector
String description = "{ any: true }"; // String | Description text selector
String displayName = "{ any: true }"; // String | Display name selector
String highIsGood = "{ any: true }"; // String | High Is Good flag selector
String iconID = "{ any: true }"; // String | Icon ID selector
String published = "{ any: true }"; // String | Published flag selector
String stackable = "{ any: true }"; // String | Stackable flag selector
String unitID = "{ any: true }"; // String | Unit ID selector
try {
    List<DgmAttributeType> result = apiInstance.getAttributeTypes(contid, maxresults, attributeID, attributeName, categoryID, defaultValue, description, displayName, highIsGood, iconID, published, stackable, unitID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DogmaApi#getAttributeTypes");
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
 **categoryID** | **String**| Category ID selector | [optional] [default to { any: true }]
 **defaultValue** | **String**| Default value selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **displayName** | **String**| Display name selector | [optional] [default to { any: true }]
 **highIsGood** | **String**| High Is Good flag selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **published** | **String**| Published flag selector | [optional] [default to { any: true }]
 **stackable** | **String**| Stackable flag selector | [optional] [default to { any: true }]
 **unitID** | **String**| Unit ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;DgmAttributeType&gt;**](DgmAttributeType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getEffects"></a>
# **getEffects**
> List&lt;DgmEffect&gt; getEffects(contid, maxresults, effectID, description, disallowAutoRepeat, dischargeAttributeID, displayName, distribution, durationAttributeID, effectCategory, effectName, electronicChance, falloffAttributeID, fittingUsageChanceAttributeID, guid, iconID, isAssistance, isOffensive, isWarpSafe, modifierInfo, npcActivationChanceAttributeID, npcUsageChanceAttributeID, postExpression, preExpression, propulsionChance, published, rangeAttributeID, rangeChance, sfxName, trackingSpeedAttributeID)

Get effects



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.DogmaApi;


DogmaApi apiInstance = new DogmaApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String effectID = "{ any: true }"; // String | Effect ID selector
String description = "{ any: true }"; // String | Description text selector
String disallowAutoRepeat = "{ any: true }"; // String | Disallow auto repeat flag selector
String dischargeAttributeID = "{ any: true }"; // String | Discharge attribute ID selector
String displayName = "{ any: true }"; // String | Display name selector
String distribution = "{ any: true }"; // String | Distribution selector
String durationAttributeID = "{ any: true }"; // String | Duration attribute ID selector
String effectCategory = "{ any: true }"; // String | Effect category selector
String effectName = "{ any: true }"; // String | Effect name selector
String electronicChance = "{ any: true }"; // String | Electronic chance selector
String falloffAttributeID = "{ any: true }"; // String | Falloff attribute ID selector
String fittingUsageChanceAttributeID = "{ any: true }"; // String | Fitting usage chance attribute ID selector
String guid = "{ any: true }"; // String | GUID selector
String iconID = "{ any: true }"; // String | Icon ID selector
String isAssistance = "{ any: true }"; // String | Is Assistance flag selector
String isOffensive = "{ any: true }"; // String | Is Offensive flag selector
String isWarpSafe = "{ any: true }"; // String | Is Warp Safe flag selector
String modifierInfo = "{ any: true }"; // String | Modifier info selector
String npcActivationChanceAttributeID = "{ any: true }"; // String | NPC activation chance attribute ID selector
String npcUsageChanceAttributeID = "{ any: true }"; // String | NPC usage chance attribute ID selector
String postExpression = "{ any: true }"; // String | Post expression selector
String preExpression = "{ any: true }"; // String | Pre expression selector
String propulsionChance = "{ any: true }"; // String | Propulsion chance selector
String published = "{ any: true }"; // String | Published flag selector
String rangeAttributeID = "{ any: true }"; // String | Range attribute ID selector
String rangeChance = "{ any: true }"; // String | Range chance selector
String sfxName = "{ any: true }"; // String | SFX name selector
String trackingSpeedAttributeID = "{ any: true }"; // String | Tracking speed attribute ID selector
try {
    List<DgmEffect> result = apiInstance.getEffects(contid, maxresults, effectID, description, disallowAutoRepeat, dischargeAttributeID, displayName, distribution, durationAttributeID, effectCategory, effectName, electronicChance, falloffAttributeID, fittingUsageChanceAttributeID, guid, iconID, isAssistance, isOffensive, isWarpSafe, modifierInfo, npcActivationChanceAttributeID, npcUsageChanceAttributeID, postExpression, preExpression, propulsionChance, published, rangeAttributeID, rangeChance, sfxName, trackingSpeedAttributeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DogmaApi#getEffects");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **effectID** | **String**| Effect ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **disallowAutoRepeat** | **String**| Disallow auto repeat flag selector | [optional] [default to { any: true }]
 **dischargeAttributeID** | **String**| Discharge attribute ID selector | [optional] [default to { any: true }]
 **displayName** | **String**| Display name selector | [optional] [default to { any: true }]
 **distribution** | **String**| Distribution selector | [optional] [default to { any: true }]
 **durationAttributeID** | **String**| Duration attribute ID selector | [optional] [default to { any: true }]
 **effectCategory** | **String**| Effect category selector | [optional] [default to { any: true }]
 **effectName** | **String**| Effect name selector | [optional] [default to { any: true }]
 **electronicChance** | **String**| Electronic chance selector | [optional] [default to { any: true }]
 **falloffAttributeID** | **String**| Falloff attribute ID selector | [optional] [default to { any: true }]
 **fittingUsageChanceAttributeID** | **String**| Fitting usage chance attribute ID selector | [optional] [default to { any: true }]
 **guid** | **String**| GUID selector | [optional] [default to { any: true }]
 **iconID** | **String**| Icon ID selector | [optional] [default to { any: true }]
 **isAssistance** | **String**| Is Assistance flag selector | [optional] [default to { any: true }]
 **isOffensive** | **String**| Is Offensive flag selector | [optional] [default to { any: true }]
 **isWarpSafe** | **String**| Is Warp Safe flag selector | [optional] [default to { any: true }]
 **modifierInfo** | **String**| Modifier info selector | [optional] [default to { any: true }]
 **npcActivationChanceAttributeID** | **String**| NPC activation chance attribute ID selector | [optional] [default to { any: true }]
 **npcUsageChanceAttributeID** | **String**| NPC usage chance attribute ID selector | [optional] [default to { any: true }]
 **postExpression** | **String**| Post expression selector | [optional] [default to { any: true }]
 **preExpression** | **String**| Pre expression selector | [optional] [default to { any: true }]
 **propulsionChance** | **String**| Propulsion chance selector | [optional] [default to { any: true }]
 **published** | **String**| Published flag selector | [optional] [default to { any: true }]
 **rangeAttributeID** | **String**| Range attribute ID selector | [optional] [default to { any: true }]
 **rangeChance** | **String**| Range chance selector | [optional] [default to { any: true }]
 **sfxName** | **String**| SFX name selector | [optional] [default to { any: true }]
 **trackingSpeedAttributeID** | **String**| Tracking speed attribute ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;DgmEffect&gt;**](DgmEffect.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getExpressions"></a>
# **getExpressions**
> List&lt;DgmExpression&gt; getExpressions(contid, maxresults, expressionID, arg1, arg2, description, expressionAttributeID, expressionGroupID, expressionName, expressionTypeID, expressionValue, operandID)

Get expressions



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.DogmaApi;


DogmaApi apiInstance = new DogmaApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String expressionID = "{ any: true }"; // String | Expression ID selector
String arg1 = "{ any: true }"; // String | First argument selector
String arg2 = "{ any: true }"; // String | Second argument selector
String description = "{ any: true }"; // String | Description text selector
String expressionAttributeID = "{ any: true }"; // String | Expression attribute ID selector
String expressionGroupID = "{ any: true }"; // String | Expression group ID selector
String expressionName = "{ any: true }"; // String | Expression name selector
String expressionTypeID = "{ any: true }"; // String | Expression type ID selector
String expressionValue = "{ any: true }"; // String | Expression value selector
String operandID = "{ any: true }"; // String | Operand ID selector
try {
    List<DgmExpression> result = apiInstance.getExpressions(contid, maxresults, expressionID, arg1, arg2, description, expressionAttributeID, expressionGroupID, expressionName, expressionTypeID, expressionValue, operandID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DogmaApi#getExpressions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **expressionID** | **String**| Expression ID selector | [optional] [default to { any: true }]
 **arg1** | **String**| First argument selector | [optional] [default to { any: true }]
 **arg2** | **String**| Second argument selector | [optional] [default to { any: true }]
 **description** | **String**| Description text selector | [optional] [default to { any: true }]
 **expressionAttributeID** | **String**| Expression attribute ID selector | [optional] [default to { any: true }]
 **expressionGroupID** | **String**| Expression group ID selector | [optional] [default to { any: true }]
 **expressionName** | **String**| Expression name selector | [optional] [default to { any: true }]
 **expressionTypeID** | **String**| Expression type ID selector | [optional] [default to { any: true }]
 **expressionValue** | **String**| Expression value selector | [optional] [default to { any: true }]
 **operandID** | **String**| Operand ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;DgmExpression&gt;**](DgmExpression.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTypeAttributes"></a>
# **getTypeAttributes**
> List&lt;DgmTypeAttribute&gt; getTypeAttributes(contid, maxresults, typeID, attributeID, valueFloat, valueInt)

Get type attributes



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.DogmaApi;


DogmaApi apiInstance = new DogmaApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String attributeID = "{ any: true }"; // String | Attribute ID selector
String valueFloat = "{ any: true }"; // String | Float value selector
String valueInt = "{ any: true }"; // String | Integer value selector
try {
    List<DgmTypeAttribute> result = apiInstance.getTypeAttributes(contid, maxresults, typeID, attributeID, valueFloat, valueInt);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DogmaApi#getTypeAttributes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **attributeID** | **String**| Attribute ID selector | [optional] [default to { any: true }]
 **valueFloat** | **String**| Float value selector | [optional] [default to { any: true }]
 **valueInt** | **String**| Integer value selector | [optional] [default to { any: true }]

### Return type

[**List&lt;DgmTypeAttribute&gt;**](DgmTypeAttribute.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTypeEffects"></a>
# **getTypeEffects**
> List&lt;DgmTypeEffect&gt; getTypeEffects(contid, maxresults, typeID, effectID, isDefault)

Get type effects



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.DogmaApi;


DogmaApi apiInstance = new DogmaApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String effectID = "{ any: true }"; // String | Effect ID selector
String isDefault = "{ any: true }"; // String | Default boolean selector
try {
    List<DgmTypeEffect> result = apiInstance.getTypeEffects(contid, maxresults, typeID, effectID, isDefault);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DogmaApi#getTypeEffects");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **effectID** | **String**| Effect ID selector | [optional] [default to { any: true }]
 **isDefault** | **String**| Default boolean selector | [optional] [default to { any: true }]

### Return type

[**List&lt;DgmTypeEffect&gt;**](DgmTypeEffect.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

