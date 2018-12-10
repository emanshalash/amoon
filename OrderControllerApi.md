# OrderControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addOrderUsingPOST**](OrderControllerApi.md#addOrderUsingPOST) | **POST** /orders/addOrder | addOrder
[**findOrderByNameUsingGET**](OrderControllerApi.md#findOrderByNameUsingGET) | **GET** /orders/orderowner | findOrderByName
[**getOrdersUsingGET**](OrderControllerApi.md#getOrdersUsingGET) | **GET** /orders/allorder | /getorders
[**sgetOrderByIDUsingGET**](OrderControllerApi.md#sgetOrderByIDUsingGET) | **GET** /orders/orderid | getOrderByID


<a name="addOrderUsingPOST"></a>
# **addOrderUsingPOST**
> String addOrderUsingPOST(name, owner)

addOrder

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.OrderControllerApi;


OrderControllerApi apiInstance = new OrderControllerApi();
String name = "name_example"; // String | name
String owner = "owner_example"; // String | owner
try {
    String result = apiInstance.addOrderUsingPOST(name, owner);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderControllerApi#addOrderUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **String**| name | [optional]
 **owner** | **String**| owner | [optional]

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="findOrderByNameUsingGET"></a>
# **findOrderByNameUsingGET**
> String findOrderByNameUsingGET(owner)

findOrderByName

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.OrderControllerApi;


OrderControllerApi apiInstance = new OrderControllerApi();
String owner = "owner_example"; // String | owner
try {
    String result = apiInstance.findOrderByNameUsingGET(owner);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderControllerApi#findOrderByNameUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **owner** | **String**| owner |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="getOrdersUsingGET"></a>
# **getOrdersUsingGET**
> List&lt;Object&gt; getOrdersUsingGET()

/getorders

This Operation retrievesall orders

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.OrderControllerApi;


OrderControllerApi apiInstance = new OrderControllerApi();
try {
    List<Object> result = apiInstance.getOrdersUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderControllerApi#getOrdersUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**List&lt;Object&gt;**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="sgetOrderByIDUsingGET"></a>
# **sgetOrderByIDUsingGET**
> OrderModelClass sgetOrderByIDUsingGET(id)

getOrderByID

This Operation retrievesa Order by its ID

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.OrderControllerApi;


OrderControllerApi apiInstance = new OrderControllerApi();
Integer id = 56; // Integer | id
try {
    OrderModelClass result = apiInstance.sgetOrderByIDUsingGET(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderControllerApi#sgetOrderByIDUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| id |

### Return type

[**OrderModelClass**](OrderModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

