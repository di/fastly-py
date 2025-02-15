# LoggingGenericCommon


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_type** | **str** | How the message should be formatted. | [optional]  if omitted the server will use the default value of "classic"
**timestamp_format** | **str, none_type** | A timestamp format | [optional] [readonly] 
**period** | **int** | How frequently log files are finalized so they can be available for reading (in seconds). | [optional]  if omitted the server will use the default value of 3600
**gzip_level** | **int** | The level of gzip encoding when sending logs (default `0`, no compression). Specifying both `compression_codec` and `gzip_level` in the same API request will result in an error. | [optional]  if omitted the server will use the default value of 0
**compression_codec** | **str** | The codec used for compressing your logs. Valid values are `zstd`, `snappy`, and `gzip`. Specifying both `compression_codec` and `gzip_level` in the same API request will result in an error. | [optional] 
**any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


