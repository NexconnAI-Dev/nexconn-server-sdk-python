# ProfanityWordListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ProfanityWordListResponseResult**](ProfanityWordListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.profanity_word_list_response import ProfanityWordListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordListResponse from a JSON string
profanity_word_list_response_instance = ProfanityWordListResponse.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordListResponse.to_json())

# convert the object into a dict
profanity_word_list_response_dict = profanity_word_list_response_instance.to_dict()
# create an instance of ProfanityWordListResponse from a dict
profanity_word_list_response_from_dict = ProfanityWordListResponse.from_dict(profanity_word_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


