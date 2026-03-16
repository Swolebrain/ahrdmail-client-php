# AHRDMail\Client\DefaultApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**checkEmailIdentityDns()**](DefaultApi.md#checkEmailIdentityDns) | **POST** /email-identity/check-dns |  |
| [**createEmailIdentity()**](DefaultApi.md#createEmailIdentity) | **POST** /email-identities |  |
| [**createSubtenant()**](DefaultApi.md#createSubtenant) | **POST** /subtenants |  |
| [**deleteEmailIdentity()**](DefaultApi.md#deleteEmailIdentity) | **DELETE** /email-identity |  |
| [**listCampaignMetrics()**](DefaultApi.md#listCampaignMetrics) | **GET** /metrics/campaigns |  |
| [**listEmailIdentities()**](DefaultApi.md#listEmailIdentities) | **GET** /email-identities |  |
| [**listSubtenantMetrics()**](DefaultApi.md#listSubtenantMetrics) | **GET** /metrics/subtenants |  |
| [**sendEmail()**](DefaultApi.md#sendEmail) | **POST** /email |  |


## `checkEmailIdentityDns()`

```php
checkEmailIdentityDns($check_email_identity_dns_request_content): \AHRDMail\Client\Model\CheckEmailIdentityDnsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$check_email_identity_dns_request_content = new \AHRDMail\Client\Model\CheckEmailIdentityDnsRequestContent(); // \AHRDMail\Client\Model\CheckEmailIdentityDnsRequestContent

try {
    $result = $apiInstance->checkEmailIdentityDns($check_email_identity_dns_request_content);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->checkEmailIdentityDns: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **check_email_identity_dns_request_content** | [**\AHRDMail\Client\Model\CheckEmailIdentityDnsRequestContent**](../Model/CheckEmailIdentityDnsRequestContent.md)|  | |

### Return type

[**\AHRDMail\Client\Model\CheckEmailIdentityDnsResponseContent**](../Model/CheckEmailIdentityDnsResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createEmailIdentity()`

```php
createEmailIdentity($create_email_identity_request_content): \AHRDMail\Client\Model\CreateEmailIdentityResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_email_identity_request_content = new \AHRDMail\Client\Model\CreateEmailIdentityRequestContent(); // \AHRDMail\Client\Model\CreateEmailIdentityRequestContent

try {
    $result = $apiInstance->createEmailIdentity($create_email_identity_request_content);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createEmailIdentity: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_email_identity_request_content** | [**\AHRDMail\Client\Model\CreateEmailIdentityRequestContent**](../Model/CreateEmailIdentityRequestContent.md)|  | |

### Return type

[**\AHRDMail\Client\Model\CreateEmailIdentityResponseContent**](../Model/CreateEmailIdentityResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createSubtenant()`

```php
createSubtenant($create_subtenant_request_content): \AHRDMail\Client\Model\CreateSubtenantResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_subtenant_request_content = new \AHRDMail\Client\Model\CreateSubtenantRequestContent(); // \AHRDMail\Client\Model\CreateSubtenantRequestContent

try {
    $result = $apiInstance->createSubtenant($create_subtenant_request_content);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createSubtenant: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_subtenant_request_content** | [**\AHRDMail\Client\Model\CreateSubtenantRequestContent**](../Model/CreateSubtenantRequestContent.md)|  | |

### Return type

[**\AHRDMail\Client\Model\CreateSubtenantResponseContent**](../Model/CreateSubtenantResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteEmailIdentity()`

```php
deleteEmailIdentity($id, $subtenant_id): \AHRDMail\Client\Model\DeleteEmailIdentityResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$subtenant_id = 'subtenant_id_example'; // string

try {
    $result = $apiInstance->deleteEmailIdentity($id, $subtenant_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteEmailIdentity: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **subtenant_id** | **string**|  | [optional] |

### Return type

[**\AHRDMail\Client\Model\DeleteEmailIdentityResponseContent**](../Model/DeleteEmailIdentityResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listCampaignMetrics()`

```php
listCampaignMetrics($subtenant_id, $next_token, $page_size): \AHRDMail\Client\Model\ListCampaignMetricsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$subtenant_id = 'subtenant_id_example'; // string
$next_token = 'next_token_example'; // string
$page_size = 3.4; // float

try {
    $result = $apiInstance->listCampaignMetrics($subtenant_id, $next_token, $page_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listCampaignMetrics: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subtenant_id** | **string**|  | |
| **next_token** | **string**|  | [optional] |
| **page_size** | **float**|  | [optional] |

### Return type

[**\AHRDMail\Client\Model\ListCampaignMetricsResponseContent**](../Model/ListCampaignMetricsResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listEmailIdentities()`

```php
listEmailIdentities($subtenant_id): \AHRDMail\Client\Model\ListEmailIdentitiesResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$subtenant_id = 'subtenant_id_example'; // string

try {
    $result = $apiInstance->listEmailIdentities($subtenant_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listEmailIdentities: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subtenant_id** | **string**|  | |

### Return type

[**\AHRDMail\Client\Model\ListEmailIdentitiesResponseContent**](../Model/ListEmailIdentitiesResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listSubtenantMetrics()`

```php
listSubtenantMetrics($next_token, $page_size): \AHRDMail\Client\Model\ListSubtenantMetricsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$next_token = 'next_token_example'; // string
$page_size = 3.4; // float

try {
    $result = $apiInstance->listSubtenantMetrics($next_token, $page_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listSubtenantMetrics: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **next_token** | **string**|  | [optional] |
| **page_size** | **float**|  | [optional] |

### Return type

[**\AHRDMail\Client\Model\ListSubtenantMetricsResponseContent**](../Model/ListSubtenantMetricsResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sendEmail()`

```php
sendEmail($send_email_request_content): \AHRDMail\Client\Model\SendEmailResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = AHRDMail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new AHRDMail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$send_email_request_content = new \AHRDMail\Client\Model\SendEmailRequestContent(); // \AHRDMail\Client\Model\SendEmailRequestContent

try {
    $result = $apiInstance->sendEmail($send_email_request_content);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sendEmail: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **send_email_request_content** | [**\AHRDMail\Client\Model\SendEmailRequestContent**](../Model/SendEmailRequestContent.md)|  | |

### Return type

[**\AHRDMail\Client\Model\SendEmailResponseContent**](../Model/SendEmailResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
