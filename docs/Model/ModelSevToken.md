# ModelSevToken

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the sevToken was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the sevToken was last updated | [optional] 
**user** | **object** | SevUser to whom the sevToken belongs | [optional] 
**token** | **string** | token of the sevUser | [optional] 
**expire** | [**\DateTime**](\DateTime.md) | expiration date of the token | [optional] 
**active** | **bool** | Defines if the token is active | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**ip_address** | **string** | Ip address of the user | [optional] 
**user_agent** | **string** | Information about the users system | [optional] 
**token_type** | **string** | Type of the token | [optional] 
**confirmation_token** | **string** | Confirmation token | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


