# ProfanityWordDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**word** | **str** | Profanity word to remove. | 

## Example

```python
from ncsdk.models.profanity_word_delete_request import ProfanityWordDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordDeleteRequest from a JSON string
profanity_word_delete_request_instance = ProfanityWordDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordDeleteRequest.to_json())

# convert the object into a dict
profanity_word_delete_request_dict = profanity_word_delete_request_instance.to_dict()
# create an instance of ProfanityWordDeleteRequest from a dict
profanity_word_delete_request_from_dict = ProfanityWordDeleteRequest.from_dict(profanity_word_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


