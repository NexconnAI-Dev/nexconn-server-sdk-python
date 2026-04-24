# AccessTokenIssueResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** | User ID that the issued access token belongs to. | [optional] 
**access_token** | **str** | Issued access token for subsequent user-authenticated requests. | [optional] 

## Example

```python
from ncsdk.models.access_token_issue_result import AccessTokenIssueResult

# TODO update the JSON string below
json = "{}"
# create an instance of AccessTokenIssueResult from a JSON string
access_token_issue_result_instance = AccessTokenIssueResult.from_json(json)
# print the JSON string representation of the object
print(AccessTokenIssueResult.to_json())

# convert the object into a dict
access_token_issue_result_dict = access_token_issue_result_instance.to_dict()
# create an instance of AccessTokenIssueResult from a dict
access_token_issue_result_from_dict = AccessTokenIssueResult.from_dict(access_token_issue_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


