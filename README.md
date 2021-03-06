# Go API client for swagger

OpenAPI for Todolist RESTful API

## Overview
This API client was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project.  By using the [swagger-spec](https://github.com/swagger-api/swagger-spec) from a remote server, you can easily generate an API client.

- API version: 1
- Package version: 1.0.0
- Build package: io.swagger.codegen.v3.generators.go.GoClientCodegen
For more information, please visit [https://github.com/IkoAfianando](https://github.com/IkoAfianando)

## Installation
Put the package under your project folder and add the following in import:
```golang
import "./swagger"
```

## Documentation for API Endpoints

All URIs are relative to *https://{environment}.programmingwithiko.com/api/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*TodolistApi* | [**TodolistGet**](docs/TodolistApi.md#todolistget) | **Get** /todolist | Get All Todolist
*TodolistApi* | [**TodolistPost**](docs/TodolistApi.md#todolistpost) | **Post** /todolist | Create New Todolist
*TodolistApi* | [**TodollistTodolistIdDelete**](docs/TodolistApi.md#todollisttodolistiddelete) | **Delete** /todollist/{todolistId} | Delete existing Todolist
*TodolistApi* | [**TodollistTodolistIdPut**](docs/TodolistApi.md#todollisttodolistidput) | **Put** /todollist/{todolistId} | Update existing Todolist

## Documentation For Models

 - [CreateOrUpdateTodolist](docs/CreateOrUpdateTodolist.md)
 - [InlineResponse200](docs/InlineResponse200.md)
 - [Todolist](docs/Todolist.md)

## Documentation For Authorization

## TodolistAuth
- **Type**: API key 

Example
```golang
auth := context.WithValue(context.Background(), sw.ContextAPIKey, sw.APIKey{
	Key: "APIKEY",
	Prefix: "Bearer", // Omit if not necessary.
})
r, err := client.Service.Operation(auth, args)
```

## Author

ikoafianando123@gmail.com
