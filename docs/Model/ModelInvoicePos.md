# ModelInvoicePos

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | creation date of the invoice position | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the invoice position was last updated | [optional] 
**invoice** | [**\Swagger\Client\Model\ModelInvoice**](ModelInvoice.md) | the Model_Invoice the invoice position belongs to | [optional] 
**part** | [**\Swagger\Client\Model\ModelPart**](ModelPart.md) | the product/part which belongs to the invoice position | [optional] 
**quantity** | **float** | the quantity of the product/part | [optional] 
**price** | **float** | the price of the product/part | [optional] 
**name** | **string** | the name of the product/part | [optional] 
**priority** | **int** |  | [optional] 
**unity** | [**\Swagger\Client\Model\ModelUnity**](ModelUnity.md) |  | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**position_number** | **int** |  | [optional] 
**text** | **string** |  | [optional] 
**discount** | **float** | does not get filled, discount is handled in the discount_model | [optional] 
**tax_rate** | **float** | tax rate in percent | [optional] 
**temporary** | **bool** |  | [optional] 
**sum_net** | **float** |  | [optional] 
**sum_gross** | **float** |  | [optional] 
**sum_discount** | **float** | does not get filled, sumDiscount is handled in the discount_model | [optional] 
**sum_tax** | **float** |  | [optional] 
**sum_net_accounting** | **float** | equals sumNet | [optional] 
**sum_tax_accounting** | **float** | equals sumTax | [optional] 
**sum_gross_accounting** | **float** | equals sumGross | [optional] 
**price_net** | **float** | net price of the product/part (one) | [optional] 
**price_gross** | **float** | gross price of the product/part (one) | [optional] 
**price_tax** | **float** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


