# Swagger\Client\StaticReferralProgramApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getStaticReferralPrograms**](StaticReferralProgramApi.md#getStaticReferralPrograms) | **GET** /StaticReferralProgram | Get staticReferralProgram list


# **getStaticReferralPrograms**
> \Swagger\Client\Model\ModelStaticReferralProgram getStaticReferralPrograms()

Get staticReferralProgram list

Calls StaticReferralProgram.php to return the staticReferralProgram list which is basically the list of referral programs.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\StaticReferralProgramApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getStaticReferralPrograms();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StaticReferralProgramApi->getStaticReferralPrograms: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\ModelStaticReferralProgram**](../Model/ModelStaticReferralProgram.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

