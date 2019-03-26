# ModelEmail

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | creation date of the Email | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the email was last updated | [optional] 
**object** | [**\Swagger\Client\Model\ModelInvoice**](ModelInvoice.md) | invoice object which is send via email | [optional] 
**from** | **string** | sender of the email | [optional] 
**to** | **string** | recipient of the email | [optional] 
**subject** | **string** | subject of the email | [optional] 
**text** | **string** | text written in the email | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**cc** | **string** | cc of the email | [optional] 
**bcc** | **string** | bcc of the email | [optional] 
**arrived** | [**\DateTime**](\DateTime.md) | arrival date of the email | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


