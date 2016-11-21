# SwaggerClient::ContactApi

All URIs are relative to *http://app.sendx.io/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**contact_identify_post**](ContactApi.md#contact_identify_post) | **POST** /contact/identify | Identify a contact as user
[**contact_track_post**](ContactApi.md#contact_track_post) | **POST** /contact/track | Add tracking info using tags to a contact


# **contact_identify_post**
> ContactResponse contact_identify_post(api_key, team_id, contact_details)

Identify a contact as user



### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::ContactApi.new

api_key = "api_key_example" # String | 

team_id = "team_id_example" # String | 

contact_details = SwaggerClient::ContactRequest.new # ContactRequest | Contact details


begin
  #Identify a contact as user
  result = api_instance.contact_identify_post(api_key, team_id, contact_details)
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling ContactApi->contact_identify_post: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **String**|  | 
 **team_id** | **String**|  | 
 **contact_details** | [**ContactRequest**](ContactRequest.md)| Contact details | 

### Return type

[**ContactResponse**](ContactResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **contact_track_post**
> TrackResponse contact_track_post(api_key, team_id, email, tag)

Add tracking info using tags to a contact



### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::ContactApi.new

api_key = "api_key_example" # String | 

team_id = "team_id_example" # String | 

email = "email_example" # String | 

tag = "tag_example" # String | 


begin
  #Add tracking info using tags to a contact
  result = api_instance.contact_track_post(api_key, team_id, email, tag)
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling ContactApi->contact_track_post: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **String**|  | 
 **team_id** | **String**|  | 
 **email** | **String**|  | 
 **tag** | **String**|  | 

### Return type

[**TrackResponse**](TrackResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



