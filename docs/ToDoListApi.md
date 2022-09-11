# {{classname}}

All URIs are relative to *http://{environment}.localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LocalhostGet**](ToDoListApi.md#LocalhostGet) | **Get** /localhost | Get All ToDoList
[**LocalhostPost**](ToDoListApi.md#LocalhostPost) | **Post** /localhost | Create New ToDoList
[**LocalhostTodolistIdDelete**](ToDoListApi.md#LocalhostTodolistIdDelete) | **Delete** /localhost/{todolistId} | Delete Existing ToDoList
[**LocalhostTodolistIdPut**](ToDoListApi.md#LocalhostTodolistIdPut) | **Put** /localhost/{todolistId} | Update Existing ToDoList

# **LocalhostGet**
> []Todolist LocalhostGet(ctx, optional)
Get All ToDoList

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ToDoListApiLocalhostGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ToDoListApiLocalhostGetOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeDone** | **optional.Bool**|  | [default to false]
 **name** | **optional.String**|  | 

### Return type

[**[]Todolist**](array.md)

### Authorization

[ToDoListAuth](../README.md#ToDoListAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **LocalhostPost**
> Todolist LocalhostPost(ctx, body)
Create New ToDoList

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**CreateOrUpdate**](CreateOrUpdate.md)|  | 

### Return type

[**Todolist**](Todolist.md)

### Authorization

[ToDoListAuth](../README.md#ToDoListAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **LocalhostTodolistIdDelete**
> bool LocalhostTodolistIdDelete(ctx, todolistId)
Delete Existing ToDoList

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **todolistId** | **string**|  | 

### Return type

**bool**

### Authorization

[ToDoListAuth](../README.md#ToDoListAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **LocalhostTodolistIdPut**
> Todolist LocalhostTodolistIdPut(ctx, body, todolistId)
Update Existing ToDoList

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**CreateOrUpdate**](CreateOrUpdate.md)|  | 
  **todolistId** | **string**|  | 

### Return type

[**Todolist**](Todolist.md)

### Authorization

[ToDoListAuth](../README.md#ToDoListAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

