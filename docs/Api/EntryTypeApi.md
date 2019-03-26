# Swagger\Client\EntryTypeApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addEntryType**](EntryTypeApi.md#addEntryType) | **POST** /EntryType | Create a new entry type
[**deleteEntryType**](EntryTypeApi.md#deleteEntryType) | **DELETE** /EntryType/{id} | Delete an existing entry type
[**entryTypeDeleteReferencedObjects**](EntryTypeApi.md#entryTypeDeleteReferencedObjects) | **DELETE** /EntryType/{id}/deleteReferencedObjects | Delete all objects bound to the specified entry type
[**getEntryTypes**](EntryTypeApi.md#getEntryTypes) | **GET** /EntryType | Get an overview of all entry types
[**updateEntryType**](EntryTypeApi.md#updateEntryType) | **PUT** /EntryType/{id} | Update an existing entry type


# **addEntryType**
> \Swagger\Client\Model\ModelEntryType addEntryType($body)

Create a new entry type

Calls EntryType.php to create an entry type

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\EntryTypeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"name=\""; // string | To create an entry type, simply enter desired values after parameter= and remove the quotation marks.

try {
    $result = $apiInstance->addEntryType($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EntryTypeApi->addEntryType: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| To create an entry type, simply enter desired values after parameter&#x3D; and remove the quotation marks. |

### Return type

[**\Swagger\Client\Model\ModelEntryType**](../Model/ModelEntryType.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteEntryType**
> deleteEntryType($id)

Delete an existing entry type

Calls EntryType.php to delete an entry type

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\EntryTypeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | id of entry type you want to delete

try {
    $apiInstance->deleteEntryType($id);
} catch (Exception $e) {
    echo 'Exception when calling EntryTypeApi->deleteEntryType: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| id of entry type you want to delete |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **entryTypeDeleteReferencedObjects**
> entryTypeDeleteReferencedObjects($id)

Delete all objects bound to the specified entry type

Tries to delete all objects bound to the specified entry type if they are not in use

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\EntryTypeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of entry type you want to use

try {
    $apiInstance->entryTypeDeleteReferencedObjects($id);
} catch (Exception $e) {
    echo 'Exception when calling EntryTypeApi->entryTypeDeleteReferencedObjects: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of entry type you want to use |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEntryTypes**
> \Swagger\Client\Model\ModelEntryType getEntryTypes($limit, $offset)

Get an overview of all entry types

Calls EntryType.php to get necessary variables.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\EntryTypeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 100; // int | Limits the number of entries returned. Default is 100
$offset = 0; // int | Set the index where the returned entry types start. Default is 0

try {
    $result = $apiInstance->getEntryTypes($limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EntryTypeApi->getEntryTypes: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Limits the number of entries returned. Default is 100 | [optional] [default to 100]
 **offset** | **int**| Set the index where the returned entry types start. Default is 0 | [optional] [default to 0]

### Return type

[**\Swagger\Client\Model\ModelEntryType**](../Model/ModelEntryType.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateEntryType**
> \Swagger\Client\Model\ModelEntryType updateEntryType($id, $body)

Update an existing entry type

Calls EntryType.php to update an entry type

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\EntryTypeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | id of entry type you want to update
$body = "body_example"; // string | Parameters which need to be updated. Please refer to the description from create entry type.    Enter the parameters according to the syntax: parameter1=&parameter2=

try {
    $result = $apiInstance->updateEntryType($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EntryTypeApi->updateEntryType: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| id of entry type you want to update |
 **body** | **string**| Parameters which need to be updated. Please refer to the description from create entry type.    Enter the parameters according to the syntax: parameter1&#x3D;&amp;parameter2&#x3D; | [optional]

### Return type

[**\Swagger\Client\Model\ModelEntryType**](../Model/ModelEntryType.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

