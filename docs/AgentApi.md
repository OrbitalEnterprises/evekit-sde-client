# AgentApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180827/api/ws/v20180827*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAgentTypes**](AgentApi.md#getAgentTypes) | **GET** /agt/agentType | Get agent types
[**getAgents**](AgentApi.md#getAgents) | **GET** /agt/agent | Get agents
[**getResearchAgents**](AgentApi.md#getResearchAgents) | **GET** /agt/researchAgent | Get research agents


<a name="getAgentTypes"></a>
# **getAgentTypes**
> List&lt;AgtAgentType&gt; getAgentTypes(contid, maxresults, agentTypeID, agentType)

Get agent types



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.AgentApi;


AgentApi apiInstance = new AgentApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String agentTypeID = "{ any: true }"; // String | Agent type ID selector
String agentType = "{ any: true }"; // String | Agent type name selector
try {
    List<AgtAgentType> result = apiInstance.getAgentTypes(contid, maxresults, agentTypeID, agentType);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AgentApi#getAgentTypes");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **agentTypeID** | **String**| Agent type ID selector | [optional] [default to { any: true }]
 **agentType** | **String**| Agent type name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;AgtAgentType&gt;**](AgtAgentType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getAgents"></a>
# **getAgents**
> List&lt;AgtAgent&gt; getAgents(contid, maxresults, agentID, agentTypeID, corporationID, divisionID, isLocator, level, locationID, quality)

Get agents



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.AgentApi;


AgentApi apiInstance = new AgentApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String agentID = "{ any: true }"; // String | Agent ID selector
String agentTypeID = "{ any: true }"; // String | Agent type ID selector
String corporationID = "{ any: true }"; // String | Corporation ID selector
String divisionID = "{ any: true }"; // String | Division ID selector
String isLocator = "{ any: true }"; // String | Locator indicator selector
String level = "{ any: true }"; // String | Level selector
String locationID = "{ any: true }"; // String | Location ID selector
String quality = "{ any: true }"; // String | Quality selector
try {
    List<AgtAgent> result = apiInstance.getAgents(contid, maxresults, agentID, agentTypeID, corporationID, divisionID, isLocator, level, locationID, quality);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AgentApi#getAgents");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **agentID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **agentTypeID** | **String**| Agent type ID selector | [optional] [default to { any: true }]
 **corporationID** | **String**| Corporation ID selector | [optional] [default to { any: true }]
 **divisionID** | **String**| Division ID selector | [optional] [default to { any: true }]
 **isLocator** | **String**| Locator indicator selector | [optional] [default to { any: true }]
 **level** | **String**| Level selector | [optional] [default to { any: true }]
 **locationID** | **String**| Location ID selector | [optional] [default to { any: true }]
 **quality** | **String**| Quality selector | [optional] [default to { any: true }]

### Return type

[**List&lt;AgtAgent&gt;**](AgtAgent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getResearchAgents"></a>
# **getResearchAgents**
> List&lt;AgtResearchAgent&gt; getResearchAgents(contid, maxresults, agentID, typeID)

Get research agents



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.AgentApi;


AgentApi apiInstance = new AgentApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String agentID = "{ any: true }"; // String | Agent ID selector
String typeID = "{ any: true }"; // String | Research type ID selector
try {
    List<AgtResearchAgent> result = apiInstance.getResearchAgents(contid, maxresults, agentID, typeID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AgentApi#getResearchAgents");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **agentID** | **String**| Agent ID selector | [optional] [default to { any: true }]
 **typeID** | **String**| Research type ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;AgtResearchAgent&gt;**](AgtResearchAgent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

