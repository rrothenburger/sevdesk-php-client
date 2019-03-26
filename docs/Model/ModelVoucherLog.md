# ModelVoucherLog

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the voucher log was created | [optional] 
**voucher** | [**\Swagger\Client\Model\ModelVoucher**](ModelVoucher.md) | voucher to which the log belongs | [optional] 
**from_status** | **int** | status of the voucher before the logged change | [optional] 
**to_status** | **int** | status of the voucher after the logged change | [optional] 
**amount_payed** | **float** | amount which was payed | [optional] 
**booking_date** | [**\DateTime**](\DateTime.md) | date of the booking | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


