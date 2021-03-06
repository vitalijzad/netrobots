# SwaggerClient::DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**board_events_get**](DefaultApi.md#board_events_get) | **GET** /board-events | 
[**board_info_get**](DefaultApi.md#board_info_get) | **GET** /board-info | 
[**robot_action_post**](DefaultApi.md#robot_action_post) | **POST** /robot-action | 
[**robot_create_post**](DefaultApi.md#robot_create_post) | **POST** /robot-create | 


# **board_events_get**
> BoardInfo board_events_get



Board Info

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

begin
  result = api_instance.board_events_get
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->board_events_get: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**BoardInfo**](BoardInfo.md)

### Authorization

No authorization required

### HTTP reuqest headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **board_info_get**
> BoardInfo board_info_get



Board Info

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

begin
  result = api_instance.board_info_get
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->board_info_get: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**BoardInfo**](BoardInfo.md)

### Authorization

No authorization required

### HTTP reuqest headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **robot_action_post**
> RobotStatus robot_action_post(command)



Send an action to a robot. The server will answer after the simulation turn is completed, and it will return the token for the next simulation turn.

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

command = SwaggerClient::RobotCommand.new # RobotCommand | 


begin
  result = api_instance.robot_action_post(command)
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->robot_action_post: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **command** | [**RobotCommand**](RobotCommand.md)|  | 

### Return type

[**RobotStatus**](RobotStatus.md)

### Authorization

No authorization required

### HTTP reuqest headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **robot_create_post**
> RobotStatus robot_create_post(configuration)



Create a new robot.

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

configuration = SwaggerClient::RobotConfiguration.new # RobotConfiguration | 


begin
  result = api_instance.robot_create_post(configuration)
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->robot_create_post: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **configuration** | [**RobotConfiguration**](RobotConfiguration.md)|  | 

### Return type

[**RobotStatus**](RobotStatus.md)

### Authorization

No authorization required

### HTTP reuqest headers

 - **Content-Type**: application/json
 - **Accept**: application/json



