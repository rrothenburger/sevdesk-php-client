# ModelPart

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the part was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the part was last updated | [optional] 
**name** | **string** | name of the part | [optional] 
**part_number** | **string** |  | [optional] 
**text** | **string** |  | [optional] 
**category** | [**\Swagger\Client\Model\ModelCategory**](ModelCategory.md) |  | [optional] 
**stock** | **float** |  | [optional] 
**unity** | [**\Swagger\Client\Model\ModelUnity**](ModelUnity.md) | unity of the part, references Unity.php | [optional] 
**price_partner** | **float** | price for a partner. Can be added via the options in the inventory where the part is displayed | [optional] 
**price_customer** | **float** | price for a customer. Can be added via the options in the inventory where the part is displayed | [optional] 
**price** | **float** | price of the part | [optional] 
**second_unity** | [**\Swagger\Client\Model\ModelUnity**](ModelUnity.md) | a second unity which can be added to the part | [optional] 
**second_unity_factor** | **float** | factor for the second unity resulting in a new sumNet for the secondUnity | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**price_purchase** | **float** |  | [optional] 
**tax_rate** | **float** |  | [optional] 
**image** | **string** |  | [optional] 
**status** | **int** |  | [optional] 
**characteristics** | **string** | characteristics of the part | [optional] 
**origin** | [**\Swagger\Client\Model\ModelPart**](ModelPart.md) |  | [optional] 
**characteristics_string** | **string** |  | [optional] 
**internal_comment** | **string** |  | [optional] 
**entry_type** | [**\Swagger\Client\Model\ModelEntryType**](ModelEntryType.md) |  | [optional] 
**accounting_type** | [**\Swagger\Client\Model\ModelAccountingType**](ModelAccountingType.md) |  | [optional] 
**price_net** | **float** |  | [optional] 
**price_gross** | **float** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


