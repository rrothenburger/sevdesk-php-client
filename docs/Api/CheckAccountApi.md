# Swagger\Client\CheckAccountApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addCheckAccount**](CheckAccountApi.md#addCheckAccount) | **POST** /CheckAccount | Create a new check account
[**checkAccountGetCurrentBalance**](CheckAccountApi.md#checkAccountGetCurrentBalance) | **GET** /CheckAccount/{id}/getCurrentBalance | Get current balance of the specified check account
[**checkAccountGetPaymentIsSupported**](CheckAccountApi.md#checkAccountGetPaymentIsSupported) | **GET** /CheckAccount/getPaymentIsSupported | Return if a payment method is supported
[**checkAccountSetDefault**](CheckAccountApi.md#checkAccountSetDefault) | **PUT** /CheckAccount/{id}/setDefault | Set the specified check accounts as the default check account
[**checkAccountTransfer**](CheckAccountApi.md#checkAccountTransfer) | **PUT** /CheckAccount/{id}/transfer | Transfer an amount from one check account to another
[**deleteCheckAccount**](CheckAccountApi.md#deleteCheckAccount) | **DELETE** /CheckAccount/{id} | Delete an existing check account
[**getCheckAccounts**](CheckAccountApi.md#getCheckAccounts) | **GET** /CheckAccount | Get an overview of all check accounts
[**updateCheckAccount**](CheckAccountApi.md#updateCheckAccount) | **PUT** /CheckAccount/{id} | Update an existing check account


# **addCheckAccount**
> \Swagger\Client\Model\ModelCheckAccount addCheckAccount($body)

Create a new check account

Calls CheckAccount.php to create a check account

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"name=&type=&currency=&status=\""; // string | To create a check account, simply enter desired values after parameter= and remove the quotation marks.

try {
    $result = $apiInstance->addCheckAccount($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->addCheckAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| To create a check account, simply enter desired values after parameter&#x3D; and remove the quotation marks. |

### Return type

[**\Swagger\Client\Model\ModelCheckAccount**](../Model/ModelCheckAccount.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkAccountGetCurrentBalance**
> checkAccountGetCurrentBalance($id)

Get current balance of the specified check account

Calls getCurrentBalance() in CheckAccount.php to get the balance of the specified check account.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of the check account of which you want the current balance

try {
    $apiInstance->checkAccountGetCurrentBalance($id);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->checkAccountGetCurrentBalance: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of the check account of which you want the current balance |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkAccountGetPaymentIsSupported**
> checkAccountGetPaymentIsSupported()

Return if a payment method is supported

Calls getPaymentIsSupported() in CheckAccount.php to get if a payment method is supported.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->checkAccountGetPaymentIsSupported();
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->checkAccountGetPaymentIsSupported: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkAccountSetDefault**
> checkAccountSetDefault($id)

Set the specified check accounts as the default check account

Calls setDefault() in CheckAccount.php to set a specified check account as the default check account

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of check account you want to set as the default check account

try {
    $apiInstance->checkAccountSetDefault($id);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->checkAccountSetDefault: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of check account you want to set as the default check account |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkAccountTransfer**
> checkAccountTransfer($id, $amount, $target_id, $target_object_name, $date)

Transfer an amount from one check account to another

Calls transfer() in CheckAccount.php to transfer an amount from one check account to another

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of check account you want to use as source account
$amount = ""; // string | Amount you want to transfer
$target_id = 56; // int | Target check account id
$target_object_name = "CheckAccount"; // string | Target check account object name
$date = ""; // string | Date of the transfer

try {
    $apiInstance->checkAccountTransfer($id, $amount, $target_id, $target_object_name, $date);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->checkAccountTransfer: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of check account you want to use as source account |
 **amount** | **string**| Amount you want to transfer | [default to ]
 **target_id** | **int**| Target check account id |
 **target_object_name** | **string**| Target check account object name | [default to CheckAccount]
 **date** | **string**| Date of the transfer | [default to ]

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteCheckAccount**
> deleteCheckAccount($id)

Delete an existing check account

Calls the delete() function in CheckAccount.php

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of check account you want to delete

try {
    $apiInstance->deleteCheckAccount($id);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->deleteCheckAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of check account you want to delete |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCheckAccounts**
> \Swagger\Client\Model\ModelDiscounts getCheckAccounts($limit, $offset, $embed)

Get an overview of all check accounts

Calls CheckAccount.php to get necessary variables.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 100; // int | Limits the number of entries returned. Default is 100
$offset = 0; // int | Set the index where the returned check accounts start. Default is 0
$embed = array("embed_example"); // string[] | Get some additional information. Embed can handle multiple values, they must be separated by comma. Default ``.

try {
    $result = $apiInstance->getCheckAccounts($limit, $offset, $embed);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->getCheckAccounts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Limits the number of entries returned. Default is 100 | [optional] [default to 100]
 **offset** | **int**| Set the index where the returned check accounts start. Default is 0 | [optional] [default to 0]
 **embed** | [**string[]**](../Model/string.md)| Get some additional information. Embed can handle multiple values, they must be separated by comma. Default &#x60;&#x60;. | [optional]

### Return type

[**\Swagger\Client\Model\ModelDiscounts**](../Model/ModelDiscounts.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateCheckAccount**
> \Swagger\Client\Model\ModelCheckAccount updateCheckAccount($id, $body)

Update an existing check account

Calls CheckAccount.php to update a check account

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\CheckAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Id of check account you want to update
$body = "body_example"; // string | Parameters which need to be updated. Please refer to the description from create discount.    Enter the parameters according to the syntax: parameter1=&parameter2=

try {
    $result = $apiInstance->updateCheckAccount($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CheckAccountApi->updateCheckAccount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of check account you want to update |
 **body** | **string**| Parameters which need to be updated. Please refer to the description from create discount.    Enter the parameters according to the syntax: parameter1&#x3D;&amp;parameter2&#x3D; | [optional]

### Return type

[**\Swagger\Client\Model\ModelCheckAccount**](../Model/ModelCheckAccount.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

