# \SmsAPI

All URIs are relative to *https://api.ubill.dev/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateBrandName**](SmsAPI.md#CreateBrandName) | **Post** /sms/brandNameCreate | Create Brand Name
[**GetDeliveryReport**](SmsAPI.md#GetDeliveryReport) | **Get** /sms/report/{smsID} | Get Delivery Report
[**GetSMSBalance**](SmsAPI.md#GetSMSBalance) | **Get** /sms/balance | Get SMS Balance
[**ListBrandNames**](SmsAPI.md#ListBrandNames) | **Get** /sms/brandNames | Get All Brand Names
[**SendSMS**](SmsAPI.md#SendSMS) | **Post** /sms/send | Send SMS



## CreateBrandName

> CreateBrandNameResponse CreateBrandName(ctx).CreateBrandNameRequest(createBrandNameRequest).Execute()

Create Brand Name



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ubill-ge/sdk-go"
)

func main() {
	createBrandNameRequest := *openapiclient.NewCreateBrandNameRequest("ubill-info") // CreateBrandNameRequest | Brand Name payload to create

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CreateBrandName(context.Background()).CreateBrandNameRequest(createBrandNameRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CreateBrandName``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBrandName`: CreateBrandNameResponse
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CreateBrandName`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateBrandNameRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createBrandNameRequest** | [**CreateBrandNameRequest**](CreateBrandNameRequest.md) | Brand Name payload to create | 

### Return type

[**CreateBrandNameResponse**](CreateBrandNameResponse.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDeliveryReport

> DeliveryReportResponse GetDeliveryReport(ctx, smsID).Execute()

Get Delivery Report



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ubill-ge/sdk-go"
)

func main() {
	smsID := int64(789) // int64 | Unique identifier of the SMS

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.GetDeliveryReport(context.Background(), smsID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.GetDeliveryReport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDeliveryReport`: DeliveryReportResponse
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.GetDeliveryReport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**smsID** | **int64** | Unique identifier of the SMS | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDeliveryReportRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DeliveryReportResponse**](DeliveryReportResponse.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSMSBalance

> SMSBalanceResponse GetSMSBalance(ctx).Execute()

Get SMS Balance



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ubill-ge/sdk-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.GetSMSBalance(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.GetSMSBalance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSMSBalance`: SMSBalanceResponse
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.GetSMSBalance`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetSMSBalanceRequest struct via the builder pattern


### Return type

[**SMSBalanceResponse**](SMSBalanceResponse.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBrandNames

> BrandNamesResponse ListBrandNames(ctx).Execute()

Get All Brand Names



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ubill-ge/sdk-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ListBrandNames(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ListBrandNames``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBrandNames`: BrandNamesResponse
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ListBrandNames`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListBrandNamesRequest struct via the builder pattern


### Return type

[**BrandNamesResponse**](BrandNamesResponse.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendSMS

> SendSMSResponse SendSMS(ctx).SendSMSRequest(sendSMSRequest).Execute()

Send SMS



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ubill-ge/sdk-go"
)

func main() {
	sendSMSRequest := *openapiclient.NewSendSMSRequest(int64(1), []int64{int64(995511194241)}, "Hello", false) // SendSMSRequest | SMS payload for sending messages

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.SendSMS(context.Background()).SendSMSRequest(sendSMSRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.SendSMS``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendSMS`: SendSMSResponse
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.SendSMS`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendSMSRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sendSMSRequest** | [**SendSMSRequest**](SendSMSRequest.md) | SMS payload for sending messages | 

### Return type

[**SendSMSResponse**](SendSMSResponse.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

