# CertificatesApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180529/api/ws/v20180529*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCertificateMasteries**](CertificatesApi.md#getCertificateMasteries) | **GET** /crt/mastery | Get certificate masteries
[**getCertificateSkills**](CertificatesApi.md#getCertificateSkills) | **GET** /crt/skill | Get certificate skills
[**getCertificates**](CertificatesApi.md#getCertificates) | **GET** /crt/certificate | Get certificates


<a name="getCertificateMasteries"></a>
# **getCertificateMasteries**
> List&lt;CrtMastery&gt; getCertificateMasteries(contid, maxresults, typeID, masteryLevel, certID)

Get certificate masteries



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CertificatesApi;


CertificatesApi apiInstance = new CertificatesApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String typeID = "{ any: true }"; // String | Type ID selector
String masteryLevel = "{ any: true }"; // String | Mastery level selector
String certID = "{ any: true }"; // String | Certificate ID selector
try {
    List<CrtMastery> result = apiInstance.getCertificateMasteries(contid, maxresults, typeID, masteryLevel, certID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CertificatesApi#getCertificateMasteries");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **typeID** | **String**| Type ID selector | [optional] [default to { any: true }]
 **masteryLevel** | **String**| Mastery level selector | [optional] [default to { any: true }]
 **certID** | **String**| Certificate ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrtMastery&gt;**](CrtMastery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getCertificateSkills"></a>
# **getCertificateSkills**
> List&lt;CrtSkill&gt; getCertificateSkills(contid, maxresults, certID, skillID, certLevelInt, skillLevel, certLevelText)

Get certificate skills



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CertificatesApi;


CertificatesApi apiInstance = new CertificatesApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String certID = "{ any: true }"; // String | Certificated ID selector
String skillID = "{ any: true }"; // String | Skill ID selector
String certLevelInt = "{ any: true }"; // String | Certificate level integer selector
String skillLevel = "{ any: true }"; // String | Skill level selector
String certLevelText = "{ any: true }"; // String | Certificate level text selector
try {
    List<CrtSkill> result = apiInstance.getCertificateSkills(contid, maxresults, certID, skillID, certLevelInt, skillLevel, certLevelText);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CertificatesApi#getCertificateSkills");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **certID** | **String**| Certificated ID selector | [optional] [default to { any: true }]
 **skillID** | **String**| Skill ID selector | [optional] [default to { any: true }]
 **certLevelInt** | **String**| Certificate level integer selector | [optional] [default to { any: true }]
 **skillLevel** | **String**| Skill level selector | [optional] [default to { any: true }]
 **certLevelText** | **String**| Certificate level text selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrtSkill&gt;**](CrtSkill.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getCertificates"></a>
# **getCertificates**
> List&lt;CrtCertificate&gt; getCertificates(contid, maxresults, certID, description, groupID, name)

Get certificates



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.CertificatesApi;


CertificatesApi apiInstance = new CertificatesApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String certID = "{ any: true }"; // String | Certificate ID selector
String description = "{ any: true }"; // String | Description selector
String groupID = "{ any: true }"; // String | Group ID selector
String name = "{ any: true }"; // String | Name selector
try {
    List<CrtCertificate> result = apiInstance.getCertificates(contid, maxresults, certID, description, groupID, name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CertificatesApi#getCertificates");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **certID** | **String**| Certificate ID selector | [optional] [default to { any: true }]
 **description** | **String**| Description selector | [optional] [default to { any: true }]
 **groupID** | **String**| Group ID selector | [optional] [default to { any: true }]
 **name** | **String**| Name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;CrtCertificate&gt;**](CrtCertificate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

