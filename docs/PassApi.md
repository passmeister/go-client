# \PassApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateOrUpdatePass**](PassApi.md#CreateOrUpdatePass) | **Post** /pass | This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.
[**DeletePass**](PassApi.md#DeletePass) | **Delete** /pass | Delete pass by pass id.
[**GetPass**](PassApi.md#GetPass) | **Get** /pass | Get pass information by pass id.
[**PassList**](PassApi.md#PassList) | **Get** /pass/list | Retrieve the list of active pass ids for a given pass type.
[**PassSync**](PassApi.md#PassSync) | **Post** /pass/sync | Send updates to all active passes for a given pass type.


# **CreateOrUpdatePass**
> CreateOrUpdatePass(ctx, passTypeId, optional)
This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **passTypeId** | [**interface{}**](.md)| your pass type id, for example P963493 (Urban Fitness) | 
 **optional** | ***PassApiCreateOrUpdatePassOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PassApiCreateOrUpdatePassOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **passId** | [**optional.Interface of interface{}**](.md)| id of the pass (provided by you when creating the pass or automatically set by passmeister) | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeletePass**
> DeletePass(ctx, passTypeId, passId)
Delete pass by pass id.

Delete pass by pass id.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **passTypeId** | [**interface{}**](.md)| your pass type id, for example P963493 (Urban Fitness) | 
  **passId** | [**interface{}**](.md)| id of the pass | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPass**
> GetPass(ctx, passTypeId, passId)
Get pass information by pass id.

Get pass information by pass id.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **passTypeId** | [**interface{}**](.md)| your pass type id, for example P963493 (Urban Fitness) | 
  **passId** | [**interface{}**](.md)| id of the pass | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PassList**
> PassList(ctx, passTypeId, optional)
Retrieve the list of active pass ids for a given pass type.

Retrieve the list of active pass ids for a given pass type.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **passTypeId** | [**interface{}**](.md)| your pass type id, for example P963493 (Urban Fitness) | 
 **optional** | ***PassApiPassListOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PassApiPassListOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | [**optional.Interface of interface{}**](.md)|  | 
 **limit** | [**optional.Interface of interface{}**](.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PassSync**
> PassSync(ctx, passTypeId)
Send updates to all active passes for a given pass type.

For example: you changed the pass type layout and now you want to update all installed passes. (The API call only confirms the scheduling of the updates, actual updating of passes on your customers devices can take a while.)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **passTypeId** | [**interface{}**](.md)| your pass type id, for example P963493 (Urban Fitness) | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

