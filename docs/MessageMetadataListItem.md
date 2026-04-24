# MessageMetadataListItem

Matches `com.rcloud.server.api.model.v4.output.MetadataItem`.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**updated_at** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.message_metadata_list_item import MessageMetadataListItem

# TODO update the JSON string below
json = "{}"
# create an instance of MessageMetadataListItem from a JSON string
message_metadata_list_item_instance = MessageMetadataListItem.from_json(json)
# print the JSON string representation of the object
print(MessageMetadataListItem.to_json())

# convert the object into a dict
message_metadata_list_item_dict = message_metadata_list_item_instance.to_dict()
# create an instance of MessageMetadataListItem from a dict
message_metadata_list_item_from_dict = MessageMetadataListItem.from_dict(message_metadata_list_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


