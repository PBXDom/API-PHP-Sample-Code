# Swagger\Client\DefaultApi

All URIs are relative to *https://api.pbxdom.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**callsGet**](DefaultApi.md#callsGet) | **GET** /Calls | 
[**featuresChartsGet**](DefaultApi.md#featuresChartsGet) | **GET** /Features/charts | 
[**featuresReportsGet**](DefaultApi.md#featuresReportsGet) | **GET** /Features/reports | 
[**featuresWidgetGet**](DefaultApi.md#featuresWidgetGet) | **GET** /Features/widget | 


# **callsGet**
> \Swagger\Client\Model\InlineResponse200[] callsGet($rpt_type, $rpt_id, $start, $limit, $sort_by, $sort_type, $from_date, $to_date, $duration, $phone, $phone1, $co, $ext, $pbx_id, $call_source, $call_type, $direction, $caller_name, $did, $dnis, $acc, $ring, $cost, $group)



Gets `Calls` info.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$rpt_type = 1.2; // double | Report type. (0 report, 1 widget, 2 chart).
$rpt_id = 1.2; // double | Report id.
$start = 3.4; // float | Start offset.
$limit = 3.4; // float | Number of results to return. Max 10K.
$sort_by = "sort_by_example"; // string | Sort column.
$sort_type = "sort_type_example"; // string | Sort mode asc/desc.
$from_date = "from_date_example"; // string | Start date time.
$to_date = "to_date_example"; // string | End date time.
$duration = 3.4; // float | Duration range.
$phone = "phone_example"; // string | List of caller phone.
$phone1 = "phone1_example"; // string | List of dialled phones.
$co = "co_example"; // string | List of trunk/co.
$ext = "ext_example"; // string | list of extensions.
$pbx_id = 3.4; // float | list of PBX Ids.
$call_source = 3.4; // float | list of callsource.
$call_type = 3.4; // float | list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls)
$direction = 3.4; // float | list of direction.(0 incoming, 1 outgoing, 2 internal)
$caller_name = "caller_name_example"; // string | list of caller name.
$did = "did_example"; // string | list of did.
$dnis = "dnis_example"; // string | list of dnis.
$acc = "acc_example"; // string | list of account code.
$ring = 3.4; // float | Ring range.Seconds unit.
$cost = 3.4; // float | Cost range.
$group = 3.4; // float | Department/Group id.

try {
    $result = $api_instance->callsGet($rpt_type, $rpt_id, $start, $limit, $sort_by, $sort_type, $from_date, $to_date, $duration, $phone, $phone1, $co, $ext, $pbx_id, $call_source, $call_type, $direction, $caller_name, $did, $dnis, $acc, $ring, $cost, $group);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->callsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rpt_type** | **double**| Report type. (0 report, 1 widget, 2 chart). |
 **rpt_id** | **double**| Report id. |
 **start** | **float**| Start offset. | [optional]
 **limit** | **float**| Number of results to return. Max 10K. | [optional]
 **sort_by** | **string**| Sort column. | [optional]
 **sort_type** | **string**| Sort mode asc/desc. | [optional]
 **from_date** | **string**| Start date time. | [optional]
 **to_date** | **string**| End date time. | [optional]
 **duration** | **float**| Duration range. | [optional]
 **phone** | **string**| List of caller phone. | [optional]
 **phone1** | **string**| List of dialled phones. | [optional]
 **co** | **string**| List of trunk/co. | [optional]
 **ext** | **string**| list of extensions. | [optional]
 **pbx_id** | **float**| list of PBX Ids. | [optional]
 **call_source** | **float**| list of callsource. | [optional]
 **call_type** | **float**| list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls) | [optional]
 **direction** | **float**| list of direction.(0 incoming, 1 outgoing, 2 internal) | [optional]
 **caller_name** | **string**| list of caller name. | [optional]
 **did** | **string**| list of did. | [optional]
 **dnis** | **string**| list of dnis. | [optional]
 **acc** | **string**| list of account code. | [optional]
 **ring** | **float**| Ring range.Seconds unit. | [optional]
 **cost** | **float**| Cost range. | [optional]
 **group** | **float**| Department/Group id. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse200[]**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **featuresChartsGet**
> \Swagger\Client\Model\InlineResponse200[] featuresChartsGet()



Gets `Charts` list.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->featuresChartsGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->featuresChartsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\InlineResponse200[]**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **featuresReportsGet**
> \Swagger\Client\Model\InlineResponse200[] featuresReportsGet()



Gets `Reports` list.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->featuresReportsGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->featuresReportsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\InlineResponse200[]**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **featuresWidgetGet**
> \Swagger\Client\Model\InlineResponse200[] featuresWidgetGet()



Gets `Widgets` list.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->featuresWidgetGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->featuresWidgetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\InlineResponse200[]**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

