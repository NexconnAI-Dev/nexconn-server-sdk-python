# UserChannelTagListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserChannelTagListResponseResult**](UserChannelTagListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_channel_tag_list_response import UserChannelTagListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagListResponse from a JSON string
user_channel_tag_list_response_instance = UserChannelTagListResponse.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagListResponse.to_json())

# convert the object into a dict
user_channel_tag_list_response_dict = user_channel_tag_list_response_instance.to_dict()
# create an instance of UserChannelTagListResponse from a dict
user_channel_tag_list_response_from_dict = UserChannelTagListResponse.from_dict(user_channel_tag_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


