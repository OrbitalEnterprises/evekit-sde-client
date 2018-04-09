# TranslationApi

All URIs are relative to *https://evekit-sde.orbital.enterprises/20180323/api/ws/v20180323*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getColumns**](TranslationApi.md#getColumns) | **GET** /trn/column | Get columns
[**getLanguages**](TranslationApi.md#getLanguages) | **GET** /trn/language | Get languages
[**getTranslations**](TranslationApi.md#getTranslations) | **GET** /trn/translation | Get translations


<a name="getColumns"></a>
# **getColumns**
> List&lt;TrnTranslationColumn&gt; getColumns(contid, maxresults, tcID, columnName, masterID, tableName, tcGroupID)

Get columns



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.TranslationApi;


TranslationApi apiInstance = new TranslationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String tcID = "{ any: true }"; // String | Translation column ID selector
String columnName = "{ any: true }"; // String | Column name selector
String masterID = "{ any: true }"; // String | Master ID selector
String tableName = "{ any: true }"; // String | Table name selector
String tcGroupID = "{ any: true }"; // String | Translation column group ID selector
try {
    List<TrnTranslationColumn> result = apiInstance.getColumns(contid, maxresults, tcID, columnName, masterID, tableName, tcGroupID);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TranslationApi#getColumns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **tcID** | **String**| Translation column ID selector | [optional] [default to { any: true }]
 **columnName** | **String**| Column name selector | [optional] [default to { any: true }]
 **masterID** | **String**| Master ID selector | [optional] [default to { any: true }]
 **tableName** | **String**| Table name selector | [optional] [default to { any: true }]
 **tcGroupID** | **String**| Translation column group ID selector | [optional] [default to { any: true }]

### Return type

[**List&lt;TrnTranslationColumn&gt;**](TrnTranslationColumn.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getLanguages"></a>
# **getLanguages**
> List&lt;TrnTranslationLanguage&gt; getLanguages(contid, maxresults, numericLanguageID, languageID, languageName)

Get languages



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.TranslationApi;


TranslationApi apiInstance = new TranslationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String numericLanguageID = "{ any: true }"; // String | Numeric language ID selector
String languageID = "{ any: true }"; // String | Language ID selector
String languageName = "{ any: true }"; // String | Language name selector
try {
    List<TrnTranslationLanguage> result = apiInstance.getLanguages(contid, maxresults, numericLanguageID, languageID, languageName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TranslationApi#getLanguages");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **numericLanguageID** | **String**| Numeric language ID selector | [optional] [default to { any: true }]
 **languageID** | **String**| Language ID selector | [optional] [default to { any: true }]
 **languageName** | **String**| Language name selector | [optional] [default to { any: true }]

### Return type

[**List&lt;TrnTranslationLanguage&gt;**](TrnTranslationLanguage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getTranslations"></a>
# **getTranslations**
> List&lt;TrnTranslation&gt; getTranslations(contid, maxresults, tcID, keyID, languageID, text)

Get translations



### Example
```java
// Import classes:
//import enterprises.orbital.evekit.sde.client.invoker.ApiException;
//import enterprises.orbital.evekit.sde.client.api.TranslationApi;


TranslationApi apiInstance = new TranslationApi();
Integer contid = -1; // Integer | Continuation ID for paged results
Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
String tcID = "{ any: true }"; // String | Translation column ID selector
String keyID = "{ any: true }"; // String | Key ID selector
String languageID = "{ any: true }"; // String | Language ID selector
String text = "{ any: true }"; // String | Text selector
try {
    List<TrnTranslation> result = apiInstance.getTranslations(contid, maxresults, tcID, keyID, languageID, text);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TranslationApi#getTranslations");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contid** | **Integer**| Continuation ID for paged results | [optional] [default to -1]
 **maxresults** | **Integer**| Maximum number of results to retrieve | [optional] [default to 1000]
 **tcID** | **String**| Translation column ID selector | [optional] [default to { any: true }]
 **keyID** | **String**| Key ID selector | [optional] [default to { any: true }]
 **languageID** | **String**| Language ID selector | [optional] [default to { any: true }]
 **text** | **String**| Text selector | [optional] [default to { any: true }]

### Return type

[**List&lt;TrnTranslation&gt;**](TrnTranslation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

