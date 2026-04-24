# UserChannelTagListItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tag_id** | **str** |  | [optional] 
**tag_name** | **str** |  | [optional] 
**created_at** | **int** | Tag creation time returned by the source API. | [optional] 

## Example

```python
from ncsdk.models.user_channel_tag_list_item import UserChannelTagListItem

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagListItem from a JSON string
user_channel_tag_list_item_instance = UserChannelTagListItem.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagListItem.to_json())

# convert the object into a dict
user_channel_tag_list_item_dict = user_channel_tag_list_item_instance.to_dict()
# create an instance of UserChannelTagListItem from a dict
user_channel_tag_list_item_from_dict = UserChannelTagListItem.from_dict(user_channel_tag_list_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


