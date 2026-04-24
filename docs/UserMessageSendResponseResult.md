# UserMessageSendResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_ids** | [**List[MessageUserDelivery]**](MessageUserDelivery.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_message_send_response_result import UserMessageSendResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserMessageSendResponseResult from a JSON string
user_message_send_response_result_instance = UserMessageSendResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserMessageSendResponseResult.to_json())

# convert the object into a dict
user_message_send_response_result_dict = user_message_send_response_result_instance.to_dict()
# create an instance of UserMessageSendResponseResult from a dict
user_message_send_response_result_from_dict = UserMessageSendResponseResult.from_dict(user_message_send_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


