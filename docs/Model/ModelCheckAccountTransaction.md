# ModelCheckAccountTransaction

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**\DateTime**](\DateTime.md) | date the check account transaction was created | [optional] 
**update** | [**\DateTime**](\DateTime.md) | date the check account transaction was last updated | [optional] 
**sev_client** | **object** | sevClient is the unique id every customer has and is used in nearly all operations | [optional] 
**value_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**entry_date** | [**\DateTime**](\DateTime.md) |  | [optional] 
**amount** | **float** | amount of the transaction | [optional] 
**gv_code** | **string** |  | [optional] 
**entry_text** | **string** |  | [optional] 
**prima_nota_no** | **string** |  | [optional] 
**paymt_purpose** | **string** |  | [optional] 
**payee_payer_bank_code** | **string** | payer bank code | [optional] 
**payee_payer_acct_no** | **string** | payer account number | [optional] 
**payee_payer_name** | **string** | payer name | [optional] 
**check_account** | [**\Swagger\Client\Model\ModelCheckAccount**](ModelCheckAccount.md) | id of the check account | [optional] 
**status** | **int** |  | [optional] 
**score** | **string** |  | [optional] 
**compare_hash** | **string** | hash to be compared | [optional] 
**entry_type** | **object** |  | [optional] 
**enshrined** | **bool** |  | [optional] 
**source_transaction** | **object** | source check account transaction used for transfers | [optional] 
**target_transaction** | **object** | destination check account transaction used for transfers | [optional] 
**obono_receipt_uuid** | **string** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


