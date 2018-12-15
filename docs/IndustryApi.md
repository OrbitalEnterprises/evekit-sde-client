# IndustryApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20181214/api/ws/v20181214*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getActivities**](IndustryApi.md#getActivities) | **GET** /ind/activity | Get industry activities
[**getActivityMaterials**](IndustryApi.md#getActivityMaterials) | **GET** /ind/activity_material | Get industry activity materials
[**getActivityProbabilities**](IndustryApi.md#getActivityProbabilities) | **GET** /ind/activity_probability | Get industry activity probabilities
[**getActivityProducts**](IndustryApi.md#getActivityProducts) | **GET** /ind/activity_product | Get industry activity products
[**getActivitySkills**](IndustryApi.md#getActivitySkills) | **GET** /ind/activity_skill | Get industry activity skills
[**getBlueprintTypes**](IndustryApi.md#getBlueprintTypes) | **GET** /ind/blueprint | Get blueprints


<a name="getActivities"></a>
# **getActivities**
> List&lt;IndActivity&gt; getActivities(contid, maxresults, typeID, activityID, time)

Get industry activities



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.IndustryApi;


IndustryApi apiInstance = new IndustryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String time = "{ any: true }"; // String | Time selector
try {
    List<IndActivity> result = apiInstance.getActivities(contid, maxresults, typeID, activityID, time);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IndustryApi#getActivities");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **time** | **String**| Time selector | [optional] [default to { any: true }]

### Return type

[**List&lt;IndActivity&gt;**](IndActivity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getActivityMaterials"></a>
# **getActivityMaterials**
> List&lt;IndActivityMaterial&gt; getActivityMaterials(contid, maxresults, typeID, activityID, materialTypeID, quantity)

Get industry activity materials



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.IndustryApi;


IndustryApi apiInstance = new IndustryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String materialTypeID = "{ any: true }"; // String | Material type ID selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<IndActivityMaterial> result = apiInstance.getActivityMaterials(contid, maxresults, typeID, activityID, materialTypeID, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IndustryApi#getActivityMaterials");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **materialTypeID** | **String**| Material type ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;IndActivityMaterial&gt;**](IndActivityMaterial.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getActivityProbabilities"></a>
# **getActivityProbabilities**
> List&lt;IndActivityProbability&gt; getActivityProbabilities(contid, maxresults, typeID, activityID, productTypeID, probability)

Get industry activity probabilities



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.IndustryApi;


IndustryApi apiInstance = new IndustryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String productTypeID = "{ any: true }"; // String | Product type ID selector
String probability = "{ any: true }"; // String | Probability selector
try {
    List<IndActivityProbability> result = apiInstance.getActivityProbabilities(contid, maxresults, typeID, activityID, productTypeID, probability);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IndustryApi#getActivityProbabilities");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **productTypeID** | **String**| Product type ID selector | [optional] [default to { any: true }]
 **probability** | **String**| Probability selector | [optional] [default to { any: true }]

### Return type

[**List&lt;IndActivityProbability&gt;**](IndActivityProbability.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getActivityProducts"></a>
# **getActivityProducts**
> List&lt;IndActivityProduct&gt; getActivityProducts(contid, maxresults, typeID, activityID, productTypeID, quantity)

Get industry activity products



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.IndustryApi;


IndustryApi apiInstance = new IndustryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String productTypeID = "{ any: true }"; // String | Product type ID selector
String quantity = "{ any: true }"; // String | Quantity selector
try {
    List<IndActivityProduct> result = apiInstance.getActivityProducts(contid, maxresults, typeID, activityID, productTypeID, quantity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IndustryApi#getActivityProducts");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **productTypeID** | **String**| Product type ID selector | [optional] [default to { any: true }]
 **quantity** | **String**| Quantity selector | [optional] [default to { any: true }]

### Return type

[**List&lt;IndActivityProduct&gt;**](IndActivityProduct.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getActivitySkills"></a>
# **getActivitySkills**
> List&lt;IndActivitySkill&gt; getActivitySkills(contid, maxresults, typeID, activityID, skillID, level)

Get industry activity skills



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.IndustryApi;


IndustryApi apiInstance = new IndustryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String activityID = "{ any: true }"; // String | Activity ID selector
String skillID = "{ any: true }"; // String | Skill ID selector
String level = "{ any: true }"; // String | Level selector
try {
    List<IndActivitySkill> result = apiInstance.getActivitySkills(contid, maxresults, typeID, activityID, skillID, level);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IndustryApi#getActivitySkills");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **activityID** | **String**| Activity ID selector | [optional] [default to { any: true }]
 **skillID** | **String**| Skill ID selector | [optional] [default to { any: true }]
 **level** | **String**| Level selector | [optional] [default to { any: true }]

### Return type

[**List&lt;IndActivitySkill&gt;**](IndActivitySkill.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getBlueprintTypes"></a>
# **getBlueprintTypes**
> List&lt;IndBlueprint&gt; getBlueprintTypes(contid, maxresults, typeID, maxProductionLimit)

Get blueprints



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.IndustryApi;


IndustryApi apiInstance = new IndustryApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String maxProductionLimit = "{ any: true }"; // String | Max production limit selector
try {
    List<IndBlueprint> result = apiInstance.getBlueprintTypes(contid, maxresults, typeID, maxProductionLimit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IndustryApi#getBlueprintTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **maxProductionLimit** | **String**| Max production limit selector | [optional] [default to { any: true }]

### Return type

[**List&lt;IndBlueprint&gt;**](IndBlueprint.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

