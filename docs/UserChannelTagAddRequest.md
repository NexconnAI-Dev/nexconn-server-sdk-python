# UserChannelTagAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**tags** | [**List[UserChannelTagItem]**](UserChannelTagItem.md) |  | 

## Example

```python
from ncsdk.models.user_channel_tag_add_request import UserChannelTagAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagAddRequest from a JSON string
user_channel_tag_add_request_instance = UserChannelTagAddRequest.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagAddRequest.to_json())

# convert the object into a dict
user_channel_tag_add_request_dict = user_channel_tag_add_request_instance.to_dict()
# create an instance of UserChannelTagAddRequest from a dict
user_channel_tag_add_request_from_dict = UserChannelTagAddRequest.from_dict(user_channel_tag_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


