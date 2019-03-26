# Swagger\Client\DocServerApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**docServerDeleteLetterPaper**](DocServerApi.md#docServerDeleteLetterPaper) | **POST** /DocServer/deleteLetterpaper | Delete a specified letter paper
[**docServerDeleteTemplate**](DocServerApi.md#docServerDeleteTemplate) | **POST** /DocServer/deleteTemplate | Delete a specified template
[**docServerGetLetterPapers**](DocServerApi.md#docServerGetLetterPapers) | **GET** /DocServer/getLetterpapers | Get an overview of all letter papers
[**docServerGetLetterPapersWithThumb**](DocServerApi.md#docServerGetLetterPapersWithThumb) | **GET** /DocServer/getLetterpapersWithThumb | Get an overview of all letter papers with their thumb
[**docServerGetTemplates**](DocServerApi.md#docServerGetTemplates) | **GET** /DocServer/getTemplates | Get an overview of all templates
[**docServerGetTemplatesWithThumb**](DocServerApi.md#docServerGetTemplatesWithThumb) | **GET** /DocServer/getTemplatesWithThumb | Get an overview of all templates with their thumb
[**docServerSetDefaultLetterPaper**](DocServerApi.md#docServerSetDefaultLetterPaper) | **POST** /DocServer/setDefaultLetterpaper | Set a letter papers as the default letter paper
[**docServerSetDefaultTemplate**](DocServerApi.md#docServerSetDefaultTemplate) | **POST** /DocServer/setDefaultTemplate | Set a template as the default template
[**docServerStoreLetterPaper**](DocServerApi.md#docServerStoreLetterPaper) | **POST** /DocServer/storeLetterpaper | Store a letter paper on the doc server
[**docServerStoreTemplate**](DocServerApi.md#docServerStoreTemplate) | **POST** /DocServer/storeTemplate | Store a template on the doc server
[**docServerTestLetterPaper**](DocServerApi.md#docServerTestLetterPaper) | **POST** /DocServer/testLetterpaper | Test a letter paper
[**docServerTestTemplate**](DocServerApi.md#docServerTestTemplate) | **POST** /DocServer/testTemplate | Test a template


# **docServerDeleteLetterPaper**
> docServerDeleteLetterPaper($body)

Delete a specified letter paper

Calls deleteLetterpaper() in DocServer.php to delete a specified letter paper

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"id=\""; // string | Enter the id of the letter paper you want to delete after id= and remove the quotation marks!

try {
    $apiInstance->docServerDeleteLetterPaper($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerDeleteLetterPaper: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the id of the letter paper you want to delete after id&#x3D; and remove the quotation marks! |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerDeleteTemplate**
> docServerDeleteTemplate($body)

Delete a specified template

Calls setDefaultTemplate() in DocServer.php to set the specified template as the default template

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"id=\""; // string | Enter the id of the template you want to set as the default template after id= and remove the quotation marks!

try {
    $apiInstance->docServerDeleteTemplate($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerDeleteTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the id of the template you want to set as the default template after id&#x3D; and remove the quotation marks! |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerGetLetterPapers**
> docServerGetLetterPapers()

Get an overview of all letter papers

Calls getLetterpapers() in DocServer.php to get the stored letter papers

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->docServerGetLetterPapers();
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerGetLetterPapers: ', $e->getMessage(), PHP_EOL;
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

# **docServerGetLetterPapersWithThumb**
> docServerGetLetterPapersWithThumb()

Get an overview of all letter papers with their thumb

Calls getLetterpapersWithThumb() in DocServer.php to get the stored letter papers with their thumb.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->docServerGetLetterPapersWithThumb();
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerGetLetterPapersWithThumb: ', $e->getMessage(), PHP_EOL;
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

# **docServerGetTemplates**
> docServerGetTemplates()

Get an overview of all templates

Calls getTemplates() in DocServer.php to get the stored templates.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->docServerGetTemplates();
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerGetTemplates: ', $e->getMessage(), PHP_EOL;
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

# **docServerGetTemplatesWithThumb**
> docServerGetTemplatesWithThumb()

Get an overview of all templates with their thumb

Calls getTemplatesWithThumb() in DocServer.php to get the stored templates with their thumb.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->docServerGetTemplatesWithThumb();
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerGetTemplatesWithThumb: ', $e->getMessage(), PHP_EOL;
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

# **docServerSetDefaultLetterPaper**
> docServerSetDefaultLetterPaper($body)

Set a letter papers as the default letter paper

Calls setDefaultLetterpaper() in DocServer.php to set the specified letter paper as the default letter paper

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"id=\""; // string | Enter the id of the letter paper you want to set as the default letter paper after id= and remove the quotation marks!

try {
    $apiInstance->docServerSetDefaultLetterPaper($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerSetDefaultLetterPaper: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the id of the letter paper you want to set as the default letter paper after id&#x3D; and remove the quotation marks! |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerSetDefaultTemplate**
> docServerSetDefaultTemplate($body)

Set a template as the default template

Calls setDefaultTemplate() in DocServer.php to set the specified template as the default template

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"id=\""; // string | Enter the id of the template you want to set as the default template after id= and remove the quotation marks!

try {
    $apiInstance->docServerSetDefaultTemplate($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerSetDefaultTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the id of the template you want to set as the default template after id&#x3D; and remove the quotation marks! |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerStoreLetterPaper**
> docServerStoreLetterPaper($body)

Store a letter paper on the doc server

Calls storeLetterpaper() in DocServer.php to store a letter paper on the doc server

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"name=&pdf=&type=null&id=null&isDefault=null\""; // string | Enter the desired values after parameter= and remove the quotation marks!    Be aware that you need to enter the base64 of the pdf you want as a letter paper after pdf=!

try {
    $apiInstance->docServerStoreLetterPaper($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerStoreLetterPaper: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the desired values after parameter&#x3D; and remove the quotation marks!    Be aware that you need to enter the base64 of the pdf you want as a letter paper after pdf&#x3D;! |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerStoreTemplate**
> docServerStoreTemplate($body)

Store a template on the doc server

Calls storeTemplate() in DocServer.php to store a template on the doc server

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"name=&html=&type=&id=null&isDefault=null&json=undefined\""; // string | Enter the desired values after parameter= and remove the quotation marks!    Be aware that you need to enter the html code of your template after html=! Type can be Invoice, Invoicereminder, Order, Contractnote, Packingllist, Letter.

try {
    $apiInstance->docServerStoreTemplate($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerStoreTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the desired values after parameter&#x3D; and remove the quotation marks!    Be aware that you need to enter the html code of your template after html&#x3D;! Type can be Invoice, Invoicereminder, Order, Contractnote, Packingllist, Letter. |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerTestLetterPaper**
> docServerTestLetterPaper($file)

Test a letter paper

Calls testLetterpaper() in DocServer.php to test your letter paper by providing the pdf.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$file = "/path/to/file.txt"; // \SplFileObject | Pdf file to test

try {
    $apiInstance->docServerTestLetterPaper($file);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerTestLetterPaper: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **\SplFileObject**| Pdf file to test |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded, multipart/form-data
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **docServerTestTemplate**
> docServerTestTemplate($body)

Test a template

Calls testTemplate() in DocServer.php to test your template by providing the html.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('token', 'Bearer');

$apiInstance = new Swagger\Client\Api\DocServerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "\"html=\""; // string | Enter the html of your template after html= and remove the quotation marks!

try {
    $apiInstance->docServerTestTemplate($body);
} catch (Exception $e) {
    echo 'Exception when calling DocServerApi->docServerTestTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string**| Enter the html of your template after html&#x3D; and remove the quotation marks! |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

