# Ahrdmail\Client\DefaultApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**checkEmailIdentityDns()**](DefaultApi.md#checkEmailIdentityDns) | **POST** /email-identity/check-dns |  |
| [**createEmailIdentity()**](DefaultApi.md#createEmailIdentity) | **POST** /email-identities |  |
| [**createMailbox()**](DefaultApi.md#createMailbox) | **POST** /mailboxes |  |
| [**createSubtenant()**](DefaultApi.md#createSubtenant) | **POST** /subtenants |  |
| [**deleteEmailIdentity()**](DefaultApi.md#deleteEmailIdentity) | **DELETE** /email-identity |  |
| [**deleteMailbox()**](DefaultApi.md#deleteMailbox) | **DELETE** /mailboxes/{address} |  |
| [**describeSubtenants()**](DefaultApi.md#describeSubtenants) | **GET** /subtenants |  |
| [**listCampaignMetrics()**](DefaultApi.md#listCampaignMetrics) | **GET** /metrics/campaigns |  |
| [**listEmailIdentities()**](DefaultApi.md#listEmailIdentities) | **GET** /email-identities |  |
| [**listMailboxes()**](DefaultApi.md#listMailboxes) | **GET** /mailboxes |  |
| [**listSubtenantMetrics()**](DefaultApi.md#listSubtenantMetrics) | **GET** /metrics/subtenants |  |
| [**sendEmail()**](DefaultApi.md#sendEmail) | **POST** /email |  |
| [**updateMailbox()**](DefaultApi.md#updateMailbox) | **PATCH** /mailboxes/{address} |  |


## `checkEmailIdentityDns()`

```php
checkEmailIdentityDns($check_email_identity_dns_request_content): \Ahrdmail\Client\Model\CheckEmailIdentityDnsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$check_email_identity_dns_request_content = new \Ahrdmail\Client\Model\CheckEmailIdentityDnsRequestContent(); // \Ahrdmail\Client\Model\CheckEmailIdentityDnsRequestContent

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
| **check_email_identity_dns_request_content** | [**\Ahrdmail\Client\Model\CheckEmailIdentityDnsRequestContent**](../Model/CheckEmailIdentityDnsRequestContent.md)|  | |

### Return type

[**\Ahrdmail\Client\Model\CheckEmailIdentityDnsResponseContent**](../Model/CheckEmailIdentityDnsResponseContent.md)

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
createEmailIdentity($create_email_identity_request_content): \Ahrdmail\Client\Model\CreateEmailIdentityResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_email_identity_request_content = new \Ahrdmail\Client\Model\CreateEmailIdentityRequestContent(); // \Ahrdmail\Client\Model\CreateEmailIdentityRequestContent

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
| **create_email_identity_request_content** | [**\Ahrdmail\Client\Model\CreateEmailIdentityRequestContent**](../Model/CreateEmailIdentityRequestContent.md)|  | |

### Return type

[**\Ahrdmail\Client\Model\CreateEmailIdentityResponseContent**](../Model/CreateEmailIdentityResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createMailbox()`

```php
createMailbox($create_mailbox_request_content): \Ahrdmail\Client\Model\CreateMailboxResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_mailbox_request_content = new \Ahrdmail\Client\Model\CreateMailboxRequestContent(); // \Ahrdmail\Client\Model\CreateMailboxRequestContent

try {
    $result = $apiInstance->createMailbox($create_mailbox_request_content);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createMailbox: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_mailbox_request_content** | [**\Ahrdmail\Client\Model\CreateMailboxRequestContent**](../Model/CreateMailboxRequestContent.md)|  | |

### Return type

[**\Ahrdmail\Client\Model\CreateMailboxResponseContent**](../Model/CreateMailboxResponseContent.md)

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
createSubtenant($create_subtenant_request_content): \Ahrdmail\Client\Model\CreateSubtenantResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_subtenant_request_content = new \Ahrdmail\Client\Model\CreateSubtenantRequestContent(); // \Ahrdmail\Client\Model\CreateSubtenantRequestContent

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
| **create_subtenant_request_content** | [**\Ahrdmail\Client\Model\CreateSubtenantRequestContent**](../Model/CreateSubtenantRequestContent.md)|  | |

### Return type

[**\Ahrdmail\Client\Model\CreateSubtenantResponseContent**](../Model/CreateSubtenantResponseContent.md)

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
deleteEmailIdentity($id, $subtenant_id): \Ahrdmail\Client\Model\DeleteEmailIdentityResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
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

[**\Ahrdmail\Client\Model\DeleteEmailIdentityResponseContent**](../Model/DeleteEmailIdentityResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteMailbox()`

```php
deleteMailbox($address, $subtenant_id): \Ahrdmail\Client\Model\DeleteMailboxResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$address = 'address_example'; // string
$subtenant_id = 'subtenant_id_example'; // string

try {
    $result = $apiInstance->deleteMailbox($address, $subtenant_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteMailbox: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **address** | **string**|  | |
| **subtenant_id** | **string**|  | |

### Return type

[**\Ahrdmail\Client\Model\DeleteMailboxResponseContent**](../Model/DeleteMailboxResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `describeSubtenants()`

```php
describeSubtenants($next_token): \Ahrdmail\Client\Model\DescribeSubtenantsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$next_token = 'next_token_example'; // string

try {
    $result = $apiInstance->describeSubtenants($next_token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->describeSubtenants: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **next_token** | **string**|  | [optional] |

### Return type

[**\Ahrdmail\Client\Model\DescribeSubtenantsResponseContent**](../Model/DescribeSubtenantsResponseContent.md)

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
listCampaignMetrics($subtenant_id, $next_token, $page_size): \Ahrdmail\Client\Model\ListCampaignMetricsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
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

[**\Ahrdmail\Client\Model\ListCampaignMetricsResponseContent**](../Model/ListCampaignMetricsResponseContent.md)

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
listEmailIdentities($subtenant_id): \Ahrdmail\Client\Model\ListEmailIdentitiesResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
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

[**\Ahrdmail\Client\Model\ListEmailIdentitiesResponseContent**](../Model/ListEmailIdentitiesResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listMailboxes()`

```php
listMailboxes($subtenant_id, $domain, $status): \Ahrdmail\Client\Model\ListMailboxesResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$subtenant_id = 'subtenant_id_example'; // string
$domain = 'domain_example'; // string | Optional. When provided, only mailboxes under this domain are returned.
$status = new \Ahrdmail\Client\Model\\Ahrdmail\Client\Model\MailboxStatus(); // \Ahrdmail\Client\Model\MailboxStatus

try {
    $result = $apiInstance->listMailboxes($subtenant_id, $domain, $status);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listMailboxes: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subtenant_id** | **string**|  | |
| **domain** | **string**| Optional. When provided, only mailboxes under this domain are returned. | [optional] |
| **status** | [**\Ahrdmail\Client\Model\MailboxStatus**](../Model/.md)|  | [optional] |

### Return type

[**\Ahrdmail\Client\Model\ListMailboxesResponseContent**](../Model/ListMailboxesResponseContent.md)

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
listSubtenantMetrics($next_token, $page_size): \Ahrdmail\Client\Model\ListSubtenantMetricsResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
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

[**\Ahrdmail\Client\Model\ListSubtenantMetricsResponseContent**](../Model/ListSubtenantMetricsResponseContent.md)

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
sendEmail($send_email_request_content): \Ahrdmail\Client\Model\SendEmailResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$send_email_request_content = new \Ahrdmail\Client\Model\SendEmailRequestContent(); // \Ahrdmail\Client\Model\SendEmailRequestContent

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
| **send_email_request_content** | [**\Ahrdmail\Client\Model\SendEmailRequestContent**](../Model/SendEmailRequestContent.md)|  | |

### Return type

[**\Ahrdmail\Client\Model\SendEmailResponseContent**](../Model/SendEmailResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateMailbox()`

```php
updateMailbox($address, $update_mailbox_request_content): \Ahrdmail\Client\Model\UpdateMailboxResponseContent
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: smithy.api.httpApiKeyAuth
$config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Ahrdmail\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');


$apiInstance = new Ahrdmail\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$address = 'address_example'; // string | Full address as returned by CreateMailbox (lowercased `<localpart>@<domain>`; for shared mailboxes includes the `+<hash>`).
$update_mailbox_request_content = new \Ahrdmail\Client\Model\UpdateMailboxRequestContent(); // \Ahrdmail\Client\Model\UpdateMailboxRequestContent

try {
    $result = $apiInstance->updateMailbox($address, $update_mailbox_request_content);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->updateMailbox: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **address** | **string**| Full address as returned by CreateMailbox (lowercased &#x60;&lt;localpart&gt;@&lt;domain&gt;&#x60;; for shared mailboxes includes the &#x60;+&lt;hash&gt;&#x60;). | |
| **update_mailbox_request_content** | [**\Ahrdmail\Client\Model\UpdateMailboxRequestContent**](../Model/UpdateMailboxRequestContent.md)|  | |

### Return type

[**\Ahrdmail\Client\Model\UpdateMailboxResponseContent**](../Model/UpdateMailboxResponseContent.md)

### Authorization

[smithy.api.httpApiKeyAuth](../../README.md#smithy.api.httpApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
