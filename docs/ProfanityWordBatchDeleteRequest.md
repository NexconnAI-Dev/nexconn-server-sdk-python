# ProfanityWordBatchDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**words** | **List[str]** | Profanity words to remove in batch. | 

## Example

```python
from ncsdk.models.profanity_word_batch_delete_request import ProfanityWordBatchDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordBatchDeleteRequest from a JSON string
profanity_word_batch_delete_request_instance = ProfanityWordBatchDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordBatchDeleteRequest.to_json())

# convert the object into a dict
profanity_word_batch_delete_request_dict = profanity_word_batch_delete_request_instance.to_dict()
# create an instance of ProfanityWordBatchDeleteRequest from a dict
profanity_word_batch_delete_request_from_dict = ProfanityWordBatchDeleteRequest.from_dict(profanity_word_batch_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


