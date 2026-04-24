# UserChannelTagItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tag_id** | **str** |  | 
**tag_name** | **str** |  | 

## Example

```python
from ncsdk.models.user_channel_tag_item import UserChannelTagItem

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagItem from a JSON string
user_channel_tag_item_instance = UserChannelTagItem.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagItem.to_json())

# convert the object into a dict
user_channel_tag_item_dict = user_channel_tag_item_instance.to_dict()
# create an instance of UserChannelTagItem from a dict
user_channel_tag_item_from_dict = UserChannelTagItem.from_dict(user_channel_tag_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


