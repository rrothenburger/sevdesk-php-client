# ModelOrderLog

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the order log was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the order was last updated | [optional] 
**date** | [**\DateTime**](\DateTime.md) | date of the order log | [optional] 
**order** | [**\Swagger\Client\Model\ModelOrder**](ModelOrder.md) | the order to which the order log refers | [optional] 
**object** | **object** | the object which was involved in the logged order action (eg. a created invoice) | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**currency** | **string** | currency of the logged order | [optional] 
**amount** | **float** | amount of the order position | [optional] 
**amount_type** | **string** | type of the order position amount, can be one from unity or custom | [optional] 
**tax_rate** | **int** | tax rate of the order | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


