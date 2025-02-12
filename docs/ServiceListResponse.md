# ServiceListResponse


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
**deleted_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
**updated_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
**comment** | **str, none_type** | A freeform descriptive note. | [optional] 
**name** | **str** | The name of the service. | [optional] 
**customer_id** | **str** | Alphanumeric string identifying the customer. | [optional] 
**type** | **str** | The type of this service. | [optional] 
**id** | **str** |  | [optional] [readonly] 
**version** | **int** | Current [version](/reference/api/services/version/) of the service. | [optional] 
**versions** | [**[SchemasVersionResponse]**](SchemasVersionResponse.md) | A list of [versions](/reference/api/services/version/) associated with the service. | [optional] 
**any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


