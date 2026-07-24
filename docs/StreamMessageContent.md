# StreamMessageContent

Stream message content payload.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** | Stream data chunk. Total message size must not exceed 128 KB across all chunks. | 
**seq** | **int** | Sequence number. Must be greater than 0, starting from 1, strictly incrementing and continuous. | 
**complete** | **bool** | Whether this is the final chunk in the stream. &#x60;true&#x60; marks the end of the stream. | 
**complete_reason** | **int** | Custom completion reason code. Only effective when &#x60;complete&#x60; is &#x60;true&#x60;. | [optional] 
**type** | **str** | Stream content type. Supported on the first chunk only. Default: text. Supported values: text, markdown, html. | [optional] 
**message_id** | **str** | Stream message unique ID. Not required for the first chunk. Required for subsequent chunks (use the value returned in the first chunk response). | [optional] 
**user** | **Dict[str, object]** | Sender user information object. Supported on the first chunk only. | [optional] 
**mentioned_info** | **Dict[str, object]** | @mention information. Supported on the first chunk only. | [optional] 
**extra** | **Dict[str, object]** | Extension information. Supported on the first chunk only. | [optional] 

## Example

```python
from ncsdk.models.stream_message_content import StreamMessageContent

# TODO update the JSON string below
json = "{}"
# create an instance of StreamMessageContent from a JSON string
stream_message_content_instance = StreamMessageContent.from_json(json)
# print the JSON string representation of the object
print(StreamMessageContent.to_json())

# convert the object into a dict
stream_message_content_dict = stream_message_content_instance.to_dict()
# create an instance of StreamMessageContent from a dict
stream_message_content_from_dict = StreamMessageContent.from_dict(stream_message_content_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


