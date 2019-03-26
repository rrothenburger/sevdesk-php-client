# ModelVoucher

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the voucher was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the voucher was last updated | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**create_user** | [**\Swagger\Client\Model\ModelSevUser**](ModelSevUser.md) | sevUser who created the voucher | [optional] 
**voucher_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**supplier** | [**\Swagger\Client\Model\ModelContact**](ModelContact.md) |  | [optional] 
**supplier_name** | **string** |  | [optional] 
**description** | **string** |  | [optional] 
**document** | [**\Swagger\Client\Model\ModelDocument**](ModelDocument.md) |  | [optional] 
**result_disdar** | **string** |  | [optional] 
**document_preview** | [**\Swagger\Client\Model\ModelDocument**](ModelDocument.md) |  | [optional] 
**pay_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**status** | **int** |  | [optional] 
**object** | **object** |  | [optional] 
**sum_net** | **float** |  | [optional] [default to 0.0]
**sum_tax** | **float** |  | [optional] [default to 0.0]
**sum_gross** | **float** |  | [optional] [default to 0.0]
**sum_net_accounting** | **float** |  | [optional] [default to 0.0]
**sum_tax_accounting** | **float** |  | [optional] [default to 0.0]
**sum_gross_accounting** | **float** |  | [optional] [default to 0.0]
**tax_type** | **string** |  | [optional] 
**credit_debit** | **string** |  | [optional] 
**hidden** | **bool** |  | [optional] 
**cost_centre** | [**\Swagger\Client\Model\ModelCostCentre**](ModelCostCentre.md) |  | [optional] 
**origin** | **object** |  | [optional] 
**voucher_type** | **string** |  | [optional] 
**recurring_intervall** | **int** |  | [optional] 
**recurring_start_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**recurring_next_voucher** | [**\DateTime**](\DateTime.md) |  | [optional] 
**recurring_last_voucher** | [**\DateTime**](\DateTime.md) |  | [optional] 
**recurring_end_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**enshrined** | **bool** |  | [optional] 
**in_source** | **string** |  | [optional] 
**tax_set** | [**\Swagger\Client\Model\ModelTaxSet**](ModelTaxSet.md) |  | [optional] 
**iban** | **string** |  | [optional] 
**accounting_special_case** | **string** |  | [optional] 
**payment_deadline** | [**\DateTime**](\DateTime.md) |  | [optional] 
**tip** | **float** |  | [optional] [default to 0.0]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


