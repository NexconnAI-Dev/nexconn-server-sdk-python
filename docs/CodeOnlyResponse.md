# CodeOnlyResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** | Return code. &#x60;0&#x60; indicates success. | 

## Example

```python
from ncsdk.models.code_only_response import CodeOnlyResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CodeOnlyResponse from a JSON string
code_only_response_instance = CodeOnlyResponse.from_json(json)
# print the JSON string representation of the object
print(CodeOnlyResponse.to_json())

# convert the object into a dict
code_only_response_dict = code_only_response_instance.to_dict()
# create an instance of CodeOnlyResponse from a dict
code_only_response_from_dict = CodeOnlyResponse.from_dict(code_only_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


