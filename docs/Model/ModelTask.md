# ModelTask

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | the date the task was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the task was last updated | [optional] 
**name** | **string** |  | [optional] 
**assigned** | [**\Swagger\Client\Model\ModelSevUser**](ModelSevUser.md) | the sevDesk user who is assigned to the task | [optional] 
**object** | **object** | can be a contact, invoice, etc to which the task refers to | [optional] 
**deadline** | [**\DateTime**](\DateTime.md) |  | [optional] 
**status** | **int** |  | [optional] 
**category** | [**\Swagger\Client\Model\ModelCategory**](ModelCategory.md) | category of the created task | [optional] 
**done** | [**\DateTime**](\DateTime.md) |  | [optional] 
**create_user** | [**\Swagger\Client\Model\ModelSevUser**](ModelSevUser.md) | the SevUser who created the task | [optional] 
**done_user** | [**\Swagger\Client\Model\ModelSevUser**](ModelSevUser.md) | the SevUser who completed the task | [optional] 
**notice_creator** | **bool** | notice the creator when the task is finished | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**begin** | [**\DateTime**](\DateTime.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


