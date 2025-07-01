# DeliveryReportItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Number** | **string** | Phone number as string | 
**StatusID** | **string** | Delivery status as string | 

## Methods

### NewDeliveryReportItem

`func NewDeliveryReportItem(number string, statusID string, ) *DeliveryReportItem`

NewDeliveryReportItem instantiates a new DeliveryReportItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeliveryReportItemWithDefaults

`func NewDeliveryReportItemWithDefaults() *DeliveryReportItem`

NewDeliveryReportItemWithDefaults instantiates a new DeliveryReportItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNumber

`func (o *DeliveryReportItem) GetNumber() string`

GetNumber returns the Number field if non-nil, zero value otherwise.

### GetNumberOk

`func (o *DeliveryReportItem) GetNumberOk() (*string, bool)`

GetNumberOk returns a tuple with the Number field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumber

`func (o *DeliveryReportItem) SetNumber(v string)`

SetNumber sets Number field to given value.


### GetStatusID

`func (o *DeliveryReportItem) GetStatusID() string`

GetStatusID returns the StatusID field if non-nil, zero value otherwise.

### GetStatusIDOk

`func (o *DeliveryReportItem) GetStatusIDOk() (*string, bool)`

GetStatusIDOk returns a tuple with the StatusID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusID

`func (o *DeliveryReportItem) SetStatusID(v string)`

SetStatusID sets StatusID field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


