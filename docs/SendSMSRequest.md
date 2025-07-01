# SendSMSRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BrandID** | **int64** | Brand identifier as integer | 
**Numbers** | **[]int64** | Array of phone numbers as integers | 
**Text** | **string** | SMS message text | 
**StopList** | **bool** | Enable/disable checking numbers in the stop list | 

## Methods

### NewSendSMSRequest

`func NewSendSMSRequest(brandID int64, numbers []int64, text string, stopList bool, ) *SendSMSRequest`

NewSendSMSRequest instantiates a new SendSMSRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendSMSRequestWithDefaults

`func NewSendSMSRequestWithDefaults() *SendSMSRequest`

NewSendSMSRequestWithDefaults instantiates a new SendSMSRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBrandID

`func (o *SendSMSRequest) GetBrandID() int64`

GetBrandID returns the BrandID field if non-nil, zero value otherwise.

### GetBrandIDOk

`func (o *SendSMSRequest) GetBrandIDOk() (*int64, bool)`

GetBrandIDOk returns a tuple with the BrandID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandID

`func (o *SendSMSRequest) SetBrandID(v int64)`

SetBrandID sets BrandID field to given value.


### GetNumbers

`func (o *SendSMSRequest) GetNumbers() []int64`

GetNumbers returns the Numbers field if non-nil, zero value otherwise.

### GetNumbersOk

`func (o *SendSMSRequest) GetNumbersOk() (*[]int64, bool)`

GetNumbersOk returns a tuple with the Numbers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumbers

`func (o *SendSMSRequest) SetNumbers(v []int64)`

SetNumbers sets Numbers field to given value.


### GetText

`func (o *SendSMSRequest) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *SendSMSRequest) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *SendSMSRequest) SetText(v string)`

SetText sets Text field to given value.


### GetStopList

`func (o *SendSMSRequest) GetStopList() bool`

GetStopList returns the StopList field if non-nil, zero value otherwise.

### GetStopListOk

`func (o *SendSMSRequest) GetStopListOk() (*bool, bool)`

GetStopListOk returns a tuple with the StopList field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStopList

`func (o *SendSMSRequest) SetStopList(v bool)`

SetStopList sets StopList field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


