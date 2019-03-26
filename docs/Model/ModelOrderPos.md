# ModelOrderPos

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | creation date of the order position | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the order position was last updated | [optional] 
**order** | [**\Swagger\Client\Model\ModelOrder**](ModelOrder.md) | Model_Order the position belongs to | [optional] 
**part** | [**\Swagger\Client\Model\ModelPart**](ModelPart.md) | The Model_Part which is used in Model_OrderPos | [optional] 
**quantity** | **float** | quantity of the Model_Part | [optional] 
**price** | **float** | price of the Model_Part | [optional] 
**name** | **string** |  | [optional] 
**priority** | **int** |  | [optional] 
**unity** | [**\Swagger\Client\Model\ModelUnity**](ModelUnity.md) |  | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**position_number** | **int** |  | [optional] 
**text** | **string** |  | [optional] 
**discount** | **float** |  | [optional] 
**optional** | **bool** |  | [optional] 
**optional_chargeable** | **bool** |  | [optional] 
**tax_rate** | **float** |  | [optional] 
**sum_net** | **float** |  | [optional] 
**sum_gross** | **float** |  | [optional] 
**sum_discount** | **float** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


