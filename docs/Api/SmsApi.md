# SiapepFrance\FreeMobile\Sms\SmsApi

All URIs are relative to *https://smsapi.free-mobile.fr/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sendmsgPost**](SmsApi.md#sendmsgPost) | **POST** /sendmsg | Send a SMS to a user

# **sendmsgPost**
> sendmsgPost($user, $pass, $msg)

Send a SMS to a user

Send a SMS to a user thanks to his credentials

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new \SiapepFrance\FreeMobile\Sms\Api\SmsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user = "user_example"; // string | User of free mobile account
$pass = "pass_example"; // string | Password of free mobile account
$msg = "msg_example"; // string | Message to send (max length 999 caracters, above it will trigger 400 error)

try {
    $apiInstance->sendmsgPost($user, $pass, $msg);
} catch (Exception $e) {
    echo 'Exception when calling SmsApi->sendmsgPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | **string**| User of free mobile account |
 **pass** | **string**| Password of free mobile account |
 **msg** | **string**| Message to send (max length 999 caracters, above it will trigger 400 error) |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

