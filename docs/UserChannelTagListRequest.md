# UserChannelTagListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 

## Example

```python
from ncsdk.models.user_channel_tag_list_request import UserChannelTagListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagListRequest from a JSON string
user_channel_tag_list_request_instance = UserChannelTagListRequest.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagListRequest.to_json())

# convert the object into a dict
user_channel_tag_list_request_dict = user_channel_tag_list_request_instance.to_dict()
# create an instance of UserChannelTagListRequest from a dict
user_channel_tag_list_request_from_dict = UserChannelTagListRequest.from_dict(user_channel_tag_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


