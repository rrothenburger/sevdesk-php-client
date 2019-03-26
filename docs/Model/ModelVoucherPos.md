# ModelVoucherPos

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the voucher positions was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the voucher position was last updated | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**voucher** | [**\Swagger\Client\Model\ModelVoucher**](ModelVoucher.md) | voucher to which the position belongs | [optional] 
**accounting_type** | [**\Swagger\Client\Model\ModelAccountingType**](ModelAccountingType.md) |  | [optional] 
**estimated_accounting_type** | [**\Swagger\Client\Model\ModelAccountingType**](ModelAccountingType.md) |  | [optional] 
**tax_rate** | **float** |  | [optional] 
**sum** | **float** |  | [optional] 
**net** | **bool** |  | [optional] 
**is_asset** | **bool** |  | [optional] 
**sum_net** | **float** |  | [optional] [default to 0.0]
**sum_tax** | **float** |  | [optional] [default to 0.0]
**sum_gross** | **float** |  | [optional] [default to 0.0]
**sum_net_accounting** | **float** |  | [optional] [default to 0.0]
**sum_tax_accounting** | **float** |  | [optional] [default to 0.0]
**sum_gross_accounting** | **float** |  | [optional] [default to 0.0]
**comment** | **string** |  | [optional] 
**is_gwg** | **bool** |  | [optional] 
**catering_tax_rate** | **float** |  | [optional] 
**catering_tip** | **float** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


