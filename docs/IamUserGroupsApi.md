# fastly.IamUserGroupsApi

All URIs are relative to *https://api.fastly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_a_user_group**](IamUserGroupsApi.md#delete_a_user_group) | **DELETE** /user-groups/{user_group_id} | Delete a user group
[**get_a_user_group**](IamUserGroupsApi.md#get_a_user_group) | **GET** /user-groups/{user_group_id} | Get a user group
[**list_user_group_members**](IamUserGroupsApi.md#list_user_group_members) | **GET** /user-groups/{user_group_id}/members | List members of a user group
[**list_user_group_roles**](IamUserGroupsApi.md#list_user_group_roles) | **GET** /user-groups/{user_group_id}/roles | List roles in a user group
[**list_user_group_service_groups**](IamUserGroupsApi.md#list_user_group_service_groups) | **GET** /user-groups/{user_group_id}/service-groups | List service groups in a user group
[**list_user_groups**](IamUserGroupsApi.md#list_user_groups) | **GET** /user-groups | List user groups


# **delete_a_user_group**
> delete_a_user_group(user_group_id)

Delete a user group

Delete a user group.

### Example

* Api Key Authentication (token):

```python
import time
import fastly
from fastly.api import iam_user_groups_api
from pprint import pprint
# Defining the host is optional and defaults to https://api.fastly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = fastly.Configuration(
    host = "https://api.fastly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: token
configuration.api_key['token'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['token'] = 'Bearer'

# Enter a context with an instance of the API client
with fastly.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = iam_user_groups_api.IamUserGroupsApi(api_client)
    user_group_id = "t4Gg2uUGZzb2W9Euo4mo0R" # str | Alphanumeric string identifying the user group.

    # example passing only required values which don't have defaults set
    try:
        # Delete a user group
        api_instance.delete_a_user_group(user_group_id)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->delete_a_user_group: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_group_id** | **str**| Alphanumeric string identifying the user group. |

### Return type

void (empty response body)

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_a_user_group**
> {str: (bool, date, datetime, dict, float, int, list, str, none_type)} get_a_user_group(user_group_id)

Get a user group

Get a user group.

### Example

* Api Key Authentication (token):

```python
import time
import fastly
from fastly.api import iam_user_groups_api
from pprint import pprint
# Defining the host is optional and defaults to https://api.fastly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = fastly.Configuration(
    host = "https://api.fastly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: token
configuration.api_key['token'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['token'] = 'Bearer'

# Enter a context with an instance of the API client
with fastly.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = iam_user_groups_api.IamUserGroupsApi(api_client)
    user_group_id = "t4Gg2uUGZzb2W9Euo4mo0R" # str | Alphanumeric string identifying the user group.

    # example passing only required values which don't have defaults set
    try:
        # Get a user group
        api_response = api_instance.get_a_user_group(user_group_id)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->get_a_user_group: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_group_id** | **str**| Alphanumeric string identifying the user group. |

### Return type

**{str: (bool, date, datetime, dict, float, int, list, str, none_type)}**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_group_members**
> {str: (bool, date, datetime, dict, float, int, list, str, none_type)} list_user_group_members(user_group_id)

List members of a user group

List members of a user group.

### Example

* Api Key Authentication (token):

```python
import time
import fastly
from fastly.api import iam_user_groups_api
from pprint import pprint
# Defining the host is optional and defaults to https://api.fastly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = fastly.Configuration(
    host = "https://api.fastly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: token
configuration.api_key['token'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['token'] = 'Bearer'

# Enter a context with an instance of the API client
with fastly.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = iam_user_groups_api.IamUserGroupsApi(api_client)
    user_group_id = "t4Gg2uUGZzb2W9Euo4mo0R" # str | Alphanumeric string identifying the user group.
    per_page = 20 # int | Number of records per page. (optional) if omitted the server will use the default value of 20
    page = 1 # int | Current page. (optional)

    # example passing only required values which don't have defaults set
    try:
        # List members of a user group
        api_response = api_instance.list_user_group_members(user_group_id)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_group_members: %s\n" % e)

    # example passing only required values which don't have defaults set
    # and optional values
    try:
        # List members of a user group
        api_response = api_instance.list_user_group_members(user_group_id, per_page=per_page, page=page)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_group_members: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_group_id** | **str**| Alphanumeric string identifying the user group. |
 **per_page** | **int**| Number of records per page. | [optional] if omitted the server will use the default value of 20
 **page** | **int**| Current page. | [optional]

### Return type

**{str: (bool, date, datetime, dict, float, int, list, str, none_type)}**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_group_roles**
> {str: (bool, date, datetime, dict, float, int, list, str, none_type)} list_user_group_roles(user_group_id)

List roles in a user group

List roles in a user group.

### Example

* Api Key Authentication (token):

```python
import time
import fastly
from fastly.api import iam_user_groups_api
from pprint import pprint
# Defining the host is optional and defaults to https://api.fastly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = fastly.Configuration(
    host = "https://api.fastly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: token
configuration.api_key['token'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['token'] = 'Bearer'

# Enter a context with an instance of the API client
with fastly.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = iam_user_groups_api.IamUserGroupsApi(api_client)
    user_group_id = "t4Gg2uUGZzb2W9Euo4mo0R" # str | Alphanumeric string identifying the user group.
    per_page = 20 # int | Number of records per page. (optional) if omitted the server will use the default value of 20
    page = 1 # int | Current page. (optional)

    # example passing only required values which don't have defaults set
    try:
        # List roles in a user group
        api_response = api_instance.list_user_group_roles(user_group_id)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_group_roles: %s\n" % e)

    # example passing only required values which don't have defaults set
    # and optional values
    try:
        # List roles in a user group
        api_response = api_instance.list_user_group_roles(user_group_id, per_page=per_page, page=page)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_group_roles: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_group_id** | **str**| Alphanumeric string identifying the user group. |
 **per_page** | **int**| Number of records per page. | [optional] if omitted the server will use the default value of 20
 **page** | **int**| Current page. | [optional]

### Return type

**{str: (bool, date, datetime, dict, float, int, list, str, none_type)}**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_group_service_groups**
> {str: (bool, date, datetime, dict, float, int, list, str, none_type)} list_user_group_service_groups(user_group_id)

List service groups in a user group

List service groups in a user group.

### Example

* Api Key Authentication (token):

```python
import time
import fastly
from fastly.api import iam_user_groups_api
from pprint import pprint
# Defining the host is optional and defaults to https://api.fastly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = fastly.Configuration(
    host = "https://api.fastly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: token
configuration.api_key['token'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['token'] = 'Bearer'

# Enter a context with an instance of the API client
with fastly.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = iam_user_groups_api.IamUserGroupsApi(api_client)
    user_group_id = "t4Gg2uUGZzb2W9Euo4mo0R" # str | Alphanumeric string identifying the user group.
    per_page = 20 # int | Number of records per page. (optional) if omitted the server will use the default value of 20
    page = 1 # int | Current page. (optional)

    # example passing only required values which don't have defaults set
    try:
        # List service groups in a user group
        api_response = api_instance.list_user_group_service_groups(user_group_id)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_group_service_groups: %s\n" % e)

    # example passing only required values which don't have defaults set
    # and optional values
    try:
        # List service groups in a user group
        api_response = api_instance.list_user_group_service_groups(user_group_id, per_page=per_page, page=page)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_group_service_groups: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_group_id** | **str**| Alphanumeric string identifying the user group. |
 **per_page** | **int**| Number of records per page. | [optional] if omitted the server will use the default value of 20
 **page** | **int**| Current page. | [optional]

### Return type

**{str: (bool, date, datetime, dict, float, int, list, str, none_type)}**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_groups**
> {str: (bool, date, datetime, dict, float, int, list, str, none_type)} list_user_groups()

List user groups

List all user groups.

### Example

* Api Key Authentication (token):

```python
import time
import fastly
from fastly.api import iam_user_groups_api
from pprint import pprint
# Defining the host is optional and defaults to https://api.fastly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = fastly.Configuration(
    host = "https://api.fastly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: token
configuration.api_key['token'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['token'] = 'Bearer'

# Enter a context with an instance of the API client
with fastly.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = iam_user_groups_api.IamUserGroupsApi(api_client)
    per_page = 20 # int | Number of records per page. (optional) if omitted the server will use the default value of 20
    page = 1 # int | Current page. (optional)

    # example passing only required values which don't have defaults set
    # and optional values
    try:
        # List user groups
        api_response = api_instance.list_user_groups(per_page=per_page, page=page)
        pprint(api_response)
    except fastly.ApiException as e:
        print("Exception when calling IamUserGroupsApi->list_user_groups: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Number of records per page. | [optional] if omitted the server will use the default value of 20
 **page** | **int**| Current page. | [optional]

### Return type

**{str: (bool, date, datetime, dict, float, int, list, str, none_type)}**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

