# Swagger\Client\AccountingSystemNumberApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addAccountingSystemNumber**](AccountingSystemNumberApi.md#addAccountingSystemNumber) | **POST** /AccountingSystemNumber | Create a new accounting system number
[**deleteAccountingSystemNumber**](AccountingSystemNumberApi.md#deleteAccountingSystemNumber) | **DELETE** /AccountingSystemNumber/{id} | Delete an existing accounting system number
[**getAccountingSystemNumbers**](AccountingSystemNumberApi.md#getAccountingSystemNumbers) | **GET** /AccountingSystemNumber | Get an overview of all accounting system numbers
[**updateAccountingSystemNumber**](AccountingSystemNumberApi.md#updateAccountingSystemNumber) | **PUT** /AccountingSystemNumber/{id} | Update an existing accounting system number


# **addAccountingSystemNumber**
> \Swagger\Client\Model\ModelAccountingSystemNumber addAccountingSystemNumber($body)

Create a new accounting system number

Calls AccountingSystemNumber.php

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\AccountingSystemNumberApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"number=&accountingType[id]=&accountingType[objectName]=AccountingType&accountingSystem[id]=1&accountingSystem[objectName]=AccountingSystem&objectName=AccountingSystemNumber  &id=&accountingSystemNumber=undefined\""; // string | To create an accounting system number, simply enter desired values after parameter= and remove the quotation marks.

try {
    $result = $apiInstance->addAccountingSystemNumber($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountingSystemNumberApi->addAccountingSystemNumber: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| To create an accounting system number, simply enter desired values after parameter&#x3D; and remove the quotation marks. |

### Return type

[**\Swagger\Client\Model\ModelAccountingSystemNumber**](../Model/ModelAccountingSystemNumber.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteAccountingSystemNumber**
> deleteAccountingSystemNumber($id)

Delete an existing accounting system number

Calls the delete() function in AccountingSystemNumber.php

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\AccountingSystemNumberApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | id of accounting system number you want to delete

try {
    $apiInstance->deleteAccountingSystemNumber($id);
} catch (Exception $e) {
    echo 'Exception when calling AccountingSystemNumberApi->deleteAccountingSystemNumber: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| id of accounting system number you want to delete |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getAccountingSystemNumbers**
> \Swagger\Client\Model\ModelAccountingSystemNumber getAccountingSystemNumbers($limit, $offset, $embed)

Get an overview of all accounting system numbers

Calls AccountingSystemNumber.php to get necessary variables.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\AccountingSystemNumberApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 1000; // int | Limits the number of entries returned. Default is 1000
$offset = 0; // int | Set the index where the returned accounting system numbers start. Default is 0
$embed = array("embed_example"); // string[] | Get some additional information. Embed can handle multiple values, they must be separated by comma. Default ``.

try {
    $result = $apiInstance->getAccountingSystemNumbers($limit, $offset, $embed);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountingSystemNumberApi->getAccountingSystemNumbers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Limits the number of entries returned. Default is 1000 | [optional] [default to 1000]
 **offset** | **int**| Set the index where the returned accounting system numbers start. Default is 0 | [optional] [default to 0]
 **embed** | [**string[]**](../Model/string.md)| Get some additional information. Embed can handle multiple values, they must be separated by comma. Default &#x60;&#x60;. | [optional]

### Return type

[**\Swagger\Client\Model\ModelAccountingSystemNumber**](../Model/ModelAccountingSystemNumber.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateAccountingSystemNumber**
> \Swagger\Client\Model\ModelAccountingType updateAccountingSystemNumber($id, $body)

Update an existing accounting system number

Calls AccountingSystemNumber.php

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\AccountingSystemNumberApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | id of accounting system number you want to update
$body = "body_example"; // string | Parameters which need to be updated. Please refer to the description from create accounting system number.    Append the parameters according to the syntax: parameter1=&parameter2= and remove the quotation marks!

try {
    $result = $apiInstance->updateAccountingSystemNumber($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountingSystemNumberApi->updateAccountingSystemNumber: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| id of accounting system number you want to update |
 **body** | **string**| Parameters which need to be updated. Please refer to the description from create accounting system number.    Append the parameters according to the syntax: parameter1&#x3D;&amp;parameter2&#x3D; and remove the quotation marks! | [optional]

### Return type

[**\Swagger\Client\Model\ModelAccountingType**](../Model/ModelAccountingType.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

