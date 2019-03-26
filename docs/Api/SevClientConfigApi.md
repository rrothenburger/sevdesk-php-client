# Swagger\Client\SevClientConfigApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getSevClientConfig**](SevClientConfigApi.md#getSevClientConfig) | **GET** /SevClientConfig | Get an overview of your sevClient config
[**updateSevClientConfig**](SevClientConfigApi.md#updateSevClientConfig) | **PUT** /SevClientConfig/{id} | Update an existing sevClient config


# **getSevClientConfig**
> \Swagger\Client\Model\ModelSevClientConfig getSevClientConfig($embed)

Get an overview of your sevClient config

Calls SevClientConfig.php to get necessary variables.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\SevClientConfigApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$embed = array("embed_example"); // string[] | Get some additional information. Embed can handle multiple values, they must be separated by comma. Default ``.

try {
    $result = $apiInstance->getSevClientConfig($embed);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SevClientConfigApi->getSevClientConfig: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **embed** | [**string[]**](../Model/string.md)| Get some additional information. Embed can handle multiple values, they must be separated by comma. Default &#x60;&#x60;. | [optional]

### Return type

[**\Swagger\Client\Model\ModelSevClientConfig**](../Model/ModelSevClientConfig.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateSevClientConfig**
> \Swagger\Client\Model\ModelSevClientConfig updateSevClientConfig($id, $body)

Update an existing sevClient config

Calls SevClientConfig.php

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\SevClientConfigApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of sevClient config you want to update
$body = "body_example"; // string | Parameters which need to be updated. Please refer to the description from create sevClient config.    Enter the parameters according to the syntax: parameter1=&parameter2=

try {
    $result = $apiInstance->updateSevClientConfig($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SevClientConfigApi->updateSevClientConfig: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of sevClient config you want to update |
 **body** | **string**| Parameters which need to be updated. Please refer to the description from create sevClient config.    Enter the parameters according to the syntax: parameter1&#x3D;&amp;parameter2&#x3D; | [optional]

### Return type

[**\Swagger\Client\Model\ModelSevClientConfig**](../Model/ModelSevClientConfig.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

