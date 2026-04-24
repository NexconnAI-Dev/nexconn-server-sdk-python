# OpenChannelMetadataEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**metadata_owner_id** | **str** | KV entry owner; serializes as &#x60;metadataOwnerId&#x60; from the source map key &#x60;userId&#x60; (&#x60;OpenChannelMetadataListResult.MetadataItem&#x60;). | [optional] 
**should_auto_delete** | **int** | Parsed from source &#x60;autoDelete&#x60; string. &#x60;1&#x60; enables auto-delete and &#x60;0&#x60; disables it. | [optional] 
**updated_at** | **int** | Parsed from source &#x60;lastSetTime&#x60; (milliseconds). | [optional] 

## Example

```python
from ncsdk.models.open_channel_metadata_entry import OpenChannelMetadataEntry

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMetadataEntry from a JSON string
open_channel_metadata_entry_instance = OpenChannelMetadataEntry.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMetadataEntry.to_json())

# convert the object into a dict
open_channel_metadata_entry_dict = open_channel_metadata_entry_instance.to_dict()
# create an instance of OpenChannelMetadataEntry from a dict
open_channel_metadata_entry_from_dict = OpenChannelMetadataEntry.from_dict(open_channel_metadata_entry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


