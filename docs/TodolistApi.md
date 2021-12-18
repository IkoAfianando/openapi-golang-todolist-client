# {{classname}}

All URIs are relative to *https://{environment}.programmingwithiko.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**TodolistGet**](TodolistApi.md#TodolistGet) | **Get** /todolist | Get All Todolist
[**TodolistPost**](TodolistApi.md#TodolistPost) | **Post** /todolist | Create New Todolist
[**TodollistTodolistIdDelete**](TodolistApi.md#TodollistTodolistIdDelete) | **Delete** /todollist/{todolistId} | Delete existing Todolist
[**TodollistTodolistIdPut**](TodolistApi.md#TodollistTodolistIdPut) | **Put** /todollist/{todolistId} | Update existing Todolist

# **TodolistGet**
> []Todolist TodolistGet(ctx, optional)
Get All Todolist

Get all todolist by default

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***TodolistApiTodolistGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a TodolistApiTodolistGetOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeDone** | **optional.Bool**| Include done todolist in the result | [default to false]
 **name** | **optional.String**| Filter todolist by name | 

### Return type

[**[]Todolist**](array.md)

### Authorization

[TodolistAuth](../README.md#TodolistAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **TodolistPost**
> Todolist TodolistPost(ctx, body)
Create New Todolist

Create new todolist to database

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**CreateOrUpdateTodolist**](CreateOrUpdateTodolist.md)|  | 

### Return type

[**Todolist**](Todolist.md)

### Authorization

[TodolistAuth](../README.md#TodolistAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **TodollistTodolistIdDelete**
> InlineResponse200 TodollistTodolistIdDelete(ctx, todolistId)
Delete existing Todolist

Delete existing todolist in database

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **todolistId** | **string**| Todolist id for updated | 

### Return type

[**InlineResponse200**](inline_response_200.md)

### Authorization

[TodolistAuth](../README.md#TodolistAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **TodollistTodolistIdPut**
> Todolist TodollistTodolistIdPut(ctx, body, todolistId)
Update existing Todolist

Update existing todolist in database

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**CreateOrUpdateTodolist**](CreateOrUpdateTodolist.md)|  | 
  **todolistId** | **string**| Todolist id for updated | 

### Return type

[**Todolist**](Todolist.md)

### Authorization

[TodolistAuth](../README.md#TodolistAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

