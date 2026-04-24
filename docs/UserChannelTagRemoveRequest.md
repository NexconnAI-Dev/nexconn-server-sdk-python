# UserChannelTagRemoveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**tag_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.user_channel_tag_remove_request import UserChannelTagRemoveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagRemoveRequest from a JSON string
user_channel_tag_remove_request_instance = UserChannelTagRemoveRequest.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagRemoveRequest.to_json())

# convert the object into a dict
user_channel_tag_remove_request_dict = user_channel_tag_remove_request_instance.to_dict()
# create an instance of UserChannelTagRemoveRequest from a dict
user_channel_tag_remove_request_from_dict = UserChannelTagRemoveRequest.from_dict(user_channel_tag_remove_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


