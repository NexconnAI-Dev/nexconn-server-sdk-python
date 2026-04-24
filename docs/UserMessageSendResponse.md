# UserMessageSendResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserMessageSendResponseResult**](UserMessageSendResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_message_send_response import UserMessageSendResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserMessageSendResponse from a JSON string
user_message_send_response_instance = UserMessageSendResponse.from_json(json)
# print the JSON string representation of the object
print(UserMessageSendResponse.to_json())

# convert the object into a dict
user_message_send_response_dict = user_message_send_response_instance.to_dict()
# create an instance of UserMessageSendResponse from a dict
user_message_send_response_from_dict = UserMessageSendResponse.from_dict(user_message_send_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


