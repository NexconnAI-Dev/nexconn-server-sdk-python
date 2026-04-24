# SingleMessageIdResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**SingleMessageIdResponseResult**](SingleMessageIdResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.single_message_id_response import SingleMessageIdResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SingleMessageIdResponse from a JSON string
single_message_id_response_instance = SingleMessageIdResponse.from_json(json)
# print the JSON string representation of the object
print(SingleMessageIdResponse.to_json())

# convert the object into a dict
single_message_id_response_dict = single_message_id_response_instance.to_dict()
# create an instance of SingleMessageIdResponse from a dict
single_message_id_response_from_dict = SingleMessageIdResponse.from_dict(single_message_id_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


