# ChannelAttributeTagItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tag_id** | **str** |  | [optional] 
**tag_name** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.channel_attribute_tag_item import ChannelAttributeTagItem

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelAttributeTagItem from a JSON string
channel_attribute_tag_item_instance = ChannelAttributeTagItem.from_json(json)
# print the JSON string representation of the object
print(ChannelAttributeTagItem.to_json())

# convert the object into a dict
channel_attribute_tag_item_dict = channel_attribute_tag_item_instance.to_dict()
# create an instance of ChannelAttributeTagItem from a dict
channel_attribute_tag_item_from_dict = ChannelAttributeTagItem.from_dict(channel_attribute_tag_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


