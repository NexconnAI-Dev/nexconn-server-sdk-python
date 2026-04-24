# AccessTokenIssueResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**AccessTokenIssueResult**](AccessTokenIssueResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.access_token_issue_response import AccessTokenIssueResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccessTokenIssueResponse from a JSON string
access_token_issue_response_instance = AccessTokenIssueResponse.from_json(json)
# print the JSON string representation of the object
print(AccessTokenIssueResponse.to_json())

# convert the object into a dict
access_token_issue_response_dict = access_token_issue_response_instance.to_dict()
# create an instance of AccessTokenIssueResponse from a dict
access_token_issue_response_from_dict = AccessTokenIssueResponse.from_dict(access_token_issue_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


