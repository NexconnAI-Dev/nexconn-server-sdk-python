# MessageMetadataSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**user_id** | **str** |  | 
**channel_type** | **int** | Supports &#x60;1&#x60; and &#x60;3&#x60;. | 
**channel_id** | **str** |  | 
**metadata** | **Dict[str, str]** | Message metadata to set. Keys support letters, digits, and &#x60;+ &#x3D; - _&#x60;, with a maximum key length of 32 characters. Each request can set up to 100 entries.  | 
**is_echo_to_sender** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.message_metadata_set_request import MessageMetadataSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MessageMetadataSetRequest from a JSON string
message_metadata_set_request_instance = MessageMetadataSetRequest.from_json(json)
# print the JSON string representation of the object
print(MessageMetadataSetRequest.to_json())

# convert the object into a dict
message_metadata_set_request_dict = message_metadata_set_request_instance.to_dict()
# create an instance of MessageMetadataSetRequest from a dict
message_metadata_set_request_from_dict = MessageMetadataSetRequest.from_dict(message_metadata_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


