# Activities

## GET/api/v1/Activitie

1. URL 

https://fakerestapi.azurewebsites.net/api/v1/Activities

2. Ожидаемый результат 
  
Тело ответа корректное, соответствует GET запросу на получение списка активностей   

HTTP status: 200 - Success

3. Заголовки запроса 

Request Headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 

нет

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```[
    {
        "id": 1,
        "title": "Activity 1",
        "dueDate": "2023-09-19T10:56:44.7649651+00:00",
        "completed": false
    },
    {
        "id": 2,
        "title": "Activity 2",
        "dueDate": "2023-09-19T11:56:44.7649676+00:00",
        "completed": true
    },
    {
        "id": 3,
        "title": "Activity 3",
        "dueDate": "2023-09-19T12:56:44.764968+00:00",
        "completed": false
    },...
]
```
## GET/api​/v1​/Activities​/5
 
1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/5

2. Ожидаемый результат 
  
Тело ответа корректное, соответствует GET запросу на получение информации об активности с id 5   

HTTP status: 200 - Success

3. Заголовки запроса 
  
Request Headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
  
нет

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
    "id": 5,
    "title": "Activity 5",
    "dueDate": "2023-09-19T15:39:11.8997047+00:00",
    "completed": false
}
]
```
## GET/api​/v1​/Activities​/0
 
1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/0

2. Ожидаемый результат 
  
Тело ответа корректное, соответствует GET запросу на получение информации об активности с id 0, которая отсутствует в каталоге   

HTTP status: 404 -  Not Found

3. Заголовки запроса 
  
Request Headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
  
нет

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
    "title": "Not Found",
    "status": 404,
    "traceId": "00-9c84bd935066b64badc1abdfd9de31a5-90aca92a7d704d4d-00"
}
```
## POST/api/v1/Activitie  

1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities

2. Ожидаемый результат 
  
Тело ответа корректное, соответствует POST запросу на добавление активности

HTTP status: 200 - Success

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{
  "id": 5,
  "title": "string",
  "dueDate": "2023-09-19T10:30:47.059Z",
  "completed": true
}
```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
  "id": 5,
  "title": "string",
  "dueDate": "2023-09-19T10:30:47.059Z",
  "completed": true
}
```  
## POST/api/v1/Activitie  

1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities

2. Ожидаемый результат 
  
Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{
  "title": "string",
  "dueDate": "2023-09-19T10:30:47.059Z",
  "completed": true
}

```  
5. Заголовки ответа
  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
``` 
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-af1cb7b1a754b649a4f21e77726fe056-4edd07c16254aa4a-00",
  "errors": {
    "$": [
      "Expected depth to be zero at the end of the JSON payload. There is an open JSON object or array that should be closed. Path: $ | LineNumber: 5 | BytePositionInLine: 0."
    ]
  }
}
```
## POST/api/v1/Activitie  

1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities

2. Ожидаемый результат 
  
Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{

  "id": f,
  "title": "string",
  "dueDate": "2023-09-19T10:30:47.059Z",
  "completed": true
}
```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
``` 
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-af1cb7b1a754b649a4f21e77726fe056-4edd07c16254aa4a-00",
  "errors": {
    "$": [
      "Expected depth to be zero at the end of the JSON payload. There is an open JSON object or array that should be closed. Path: $ | LineNumber: 5 | BytePositionInLine: 0."
    ]
  }
}
```
## POST/api/v1/Activitie  

1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities

2. Ожидаемый результат 
  
Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 415 Unsupported Media Type

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```

```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
``` 
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title": "Unsupported Media Type",
    "status": 415,
    "traceId": "00-1946b2c84ab66a4f9e358983a40e328e-19eb552b03331f40-00"
}
```
## PUT/api​/v1​/Activities​/5
  
1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/5

2. Ожидаемый результат 
  
Тело ответа корректное, соответствует PUT запросу на изменение информации об активности с id 5   

HTTP status: 200 - Success

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-09-19T14:52:29.114Z",
  "completed": true
}
```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-09-19T14:52:29.114Z",
  "completed": true
}

```
## PUT/api​/v1​/Activities​/5
  
1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/5

2. Ожидаемый результат 
  
Тело ответа содержит сообщение о том, что допущена ошибка, указан ее статус и значение

HTTP status: 400 Bad Request

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{
    "id": 0,
    "title": "string",
    "dueDate": "2023-09-19T14:52:29.114Z",
...
}
```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-04dd6518e32b984fa09394c0f74edf53-8b89ee5768523f4d-00",
    "errors": {
        "$": [
            "Expected start of a property name or value, but instead reached end of data. Path: $ | LineNumber: 4 | BytePositionInLine: 0."
        ]
    }
}
```
## PUT/api​/v1​/Activities​/5
  
1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/5

2. Ожидаемый результат 
  
Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status:415 Unsupported Media Type

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title": "Unsupported Media Type",
    "status": 415,
    "traceId": "00-b847bccf3e40564994744656827631c3-98bfdb2731ba814b-00"
}
```
## PUT/api​/v1​/Activities​/10000000000 

1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/10000000000

2. Ожидаемый результат 
  
Тело ответа содержит сообщение о том, что допущена ошибка, указан ее статус и значение

HTTP status: 400 Bad Request

3. Заголовки запроса 
  
Request Headers
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-09-19T14:52:29.114Z",
  "completed": true
}
```  
5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-adeb27d9c8fb1c4ebe328b7686251224-bd82351b52f03544-00",
    "errors": {
        "id": [
            "The value '10000000000' is not valid."
        ]
    }
}
```
## DELETE/api​/v1​/Activities​/5

1. URL  

https://fakerestapi.azurewebsites.net/api/v1/Activities/5

2. Ожидаемый результат 
  
HTTP status: 200 - Success

3. Заголовки запроса 
  
Request Headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b3e448ea-d60b-4bb3-9fcd-b5daea5e93ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
  
нет

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
HTTP status: 200 - Success
```
# Authors

## GET/api​/v1​/Authors

1. https://fakerestapi.azurewebsites.net/api/v1/Authors

2. Тело ответа корректное, соответствует GET запросу на получение списка авторов 
HTTP status: 200 - Sucсess

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: ac8f1451-03bb-4170-8de6-c922bbf9ef2b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Request body 

нет

5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 09:29:34 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Response body 
```
[
    {
        "id":1,
        "idBook":1,
        "firstName":"First Name 1",
        "lastName":"Last Name 1"
    },
    {
        "id":2,
        "idBook":1,
        "firstName":"First Name 2",
        "lastName":"Last Name 2"
    },
    {
        "id":3,"idBook":1,
        "firstName":"First Name 3",
        "lastName":"Last Name 3"
    },
    ...
]
```

## GET/api​/v1​/Authors​/authors​/books​/{idBook}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/5

2. Тело ответа корректное, соответствует GET запросу на получение информации о конкретной книги автора
HTTP status: 200 - Sucсess

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 43b12b49-2868-4716-b839-e29b833a2429
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Request body 
```
[
    {
        "id": 13,
        "idBook": 5,
        "firstName": "First Name 13",
        "lastName": "Last Name 13"
    },
    ...
]
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 11:23:41 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body 
```
[
    {
        "id":13,"idBook":5,
        "firstName":"First Name 13",
        "lastName":"Last Name 13"
        },
        {
        "id":14,
        "idBook":5,
        "firstName":"First Name 14",
        "lastName":"Last Name 14"
        },
        {
        "id":15,
        "idBook":5,
        "firstName":"First Name 15",
        "lastName":"Last Name 15"
        },
        {
        "id":16,
        "idBook":5,
        "firstName":"First Name 16",
        "lastName":"Last Name 16"
        }
        ]
```

## GET/api​/v1​/Authors​/authors​/books​/{idBook}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/10000000000

2. Тело ответа корректное, соответствует GET запросу на получение информации о книге с id "10000000000"
HTTP status: 400 Error: Bad Request

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 822900d4-2ea9-4f7c-9c10-853cc54cef13
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Request body 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-e9b19d61fca0dc45a7405292d95a9607-fd6294c9117ede4c-00",
    "errors": {
        "idBook": [
            "The value '10000000000' is not valid."
        ]
    }
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 13:28:11 GMT
Server: Kestrel
Transfer-Encoding: chunked
```

6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title":"One or more validation errors occurred.",
    "status":400,"traceId":"00-e9b19d61fca0dc45a7405292d95a9607-fd6294c9117ede4c-00",
    "errors":
    {
    "idBook":["The value '10000000000' is not valid."]
    }
}
```

## GET/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/5 

2. Тело ответа корректное, соответствует GET запросу на получение информации об авторах с id 5
HTTP status: 200 - Sucсess

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 7d3658d4-2d08-46dc-9467-2ce9a0f329cb
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Request body 
```
{
    "id": 5,
    "idBook": 2,
    "firstName": "First Name 5",
    "lastName": "Last Name 5"
}
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 13:42:21 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Response body 
```
{
    "id":5,
    "idBook":2,
    "firstName":"First Name 5",
    "lastName":"Last Name 5"
}
```

## GET/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/10000000000 

2. Тело ответа корректное, соответствует GET-запросу о конкретном авторе с id "10000000000"
HTTP status: 400 Error Bad Request

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: bb698e92-8319-43a8-86c8-2a69b2bda305
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Request body 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-b65276c5bf69d249a8a6ea1d20867c07-78ba963781fda444-00",
    "errors": {
        "id": [
            "The value '10000000000' is not valid."
        ]
    }
}
```

5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 13:47:35 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title":"One or more validation errors occurred.",
    "status":400,
    "traceId":"00-b65276c5bf69d249a8a6ea1d20867c07-78ba963781fda444-00",
    "errors":{"id":["The value '10000000000' is not valid."]}
}
``` 

## POST/api​/v1​/Authors

1. https://fakerestapi.azurewebsites.net/api/v1/Authors

2. Тело ответа корректное, соответствует POST-запросу на создание нового автора
HTTP status: 200 - Sucсess

3. Request headers 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 3d0a6d87-52b5-4867-b336-3bb486fa166c
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 
```
{
  "id": 5,
  "idBook": 6,
  "firstName": "Hot",
  "lastName": "Pepper"
}
```

5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 13:55:28 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body 
```
{
    "id":5,
    "idBook":6,
    "firstName":"Hot",
    "lastName":"Pepper"
}
```

## POST/api​/v1​/Authors

1. https://fakerestapi.azurewebsites.net/api/v1/Authors 

2. Тело ответа корректное, соответствует введенному невалидному id автора
HTTP status: 400 Error Bad Request

3. Request headers 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: a608f16e-97f3-4164-a338-7fa85568e721
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Request body 
```
{
  "id": crazy,
  "idBook": 6,
  "firstName": "Hot",
  "lastName": "Pepper"
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 14:02:37 GMT
Server: Kestrel
Transfer-Encoding: chunked
```

6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title":"One or more validation errors occurred.",
    "status":400,"traceId":"00-4818c349c2dbb64798fef52d1ccd25b5-73fa60111c2f9842-00",
    "errors":{"$.id":["'c' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."]}
}
```

## POST/api​/v1​/Authors

1. https://fakerestapi.azurewebsites.net/api/v1/Authors 

2. Тело ответа корректное, соответствует введенному пустому запросу
HTTP status: 415 Unsupported Media Type

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: f545aad8-54b2-459e-8e62-75359dc19d53
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 

нет

5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 14:16:17 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title":"Unsupported Media Type","status":415,
    "traceId":"00-0fabae03bf20bb43b651fb5736d5cb09-5d5de20119aee64d-00"
    }
```
## POST/api​/v1​/Authors

1. https://fakerestapi.azurewebsites.net/api/v1/Authors

2. Тело ответа корректное, соответствует неверно введенному запросу 
HTTP status: 400 Error Bad Request

3. Request headers 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: aac7abe7-074f-4642-9fbf-18d4893cbafe
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 
```
{
  "id": 0,
  "idBook": 0,
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 14:25:11 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title":"One or more validation errors occurred.",
    "status":400,
    "traceId":"00-9a68f9c4b3ff16478f1594d93dcc1fdb-e76ab5de176b6b4c-00",
    "errors":{"$":["The JSON object contains a trailing comma at the end which is not supported in this mode. Change the reader options. Path: $ | LineNumber: 3 | BytePositionInLine: 0."]}
}
```
## PUT/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/5

2. Тело ответа корректное, соответствует введенным данным
HTTP status: 200 - Sucсess

3. Request headers 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: d78a1f05-5697-4590-a245-2c978065cb19
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 
```
{
  "id": 5,
  "idBook": 5,
  "firstName": "Hot",
  "lastName": "Pepper"
}
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 14:30:18 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body 
```
{
    "id":5,
    "idBook":5,
    "firstName":"Hot",
    "lastName":"Pepper"
}
```
## PUT/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/5

2. Тело ответа корректное, соответствует введенным некорректно данным
HTTP status: 400 Error Bad Request

3. Request headers 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: d2c07f69-f10a-4cdf-874b-58eb4dc220d8
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 
```
{
  "id": 5,
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 14:35:18 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title":"One or more validation errors occurred.","status":400,
    "traceId":"00-82f48459c3068447a9dbebc9a8534ef2-b052e7ba2e57664b-00",
    "errors":{"$":["The JSON object contains a trailing comma at the end which is not supported in this mode. Change the reader options. Path: $ | LineNumber: 2 | BytePositionInLine: 0."]}
}
```
## PUT/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/5

2. Тело ответа корректное, соответствует запросу с пустым телом
HTTP status: 415 Unsupported Media Type

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 17bccb20-b5bc-4311-86a4-ad9c06ea6aad
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 

нет

5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 14:39:36 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title":"Unsupported Media Type",
    "status":415,"traceId":"00-c0363fe07370b04c99c284eada7075b5-7832008ba9b3de44-00"
}
```
## PUT/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/5

2. Тело ответа корректное, соответствует введенному неверно id
HTTP status: 400 Error Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 31f47915-0225-4598-b725-57ecb5e75886
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 
```
{
  "id": crazy,
  "idBook": 0,
  "firstName": "string",3
  "lastName": "string"
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 21 Sep 2023 14:45:19 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body 
```
{
    "type":"https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title":"One or more validation errors occurred.",
    "status":400,
    "traceId":"00-ebef3f93bc592f428f8e2fb6f49acae2-f692ec4c5804034d-00",
    "errors":{"$.id":["'c' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."]}
}
```
## DELETE/api​/v1​/Authors​/{id}

1. https://fakerestapi.azurewebsites.net/api/v1/Authors/5

2. Ожидаемый результат:
HTTP status: 200 - Sucсess

3. Request headers 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 17c0abc7-6a5a-4555-9b2c-6ba0826a49f6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body 

нет

5. Response headers
```
Content-Length: 0
Date: Thu, 21 Sep 2023 14:54:14 GMT
Server: Kestrel
api-supported-versions: 1.0
```
6. Response body 

нет

# Books   

## GET​/api​/v1​/Books  

1. URL   

https://fakerestapi.azurewebsites.net/api/v1/Books   

2. Ожидаемый результат   

Тело ответа корректное, соответствует GET запросу на получение списка авторов  

HTTP status: 200 - Sucсess   

3. Заголовки запроса - Request headers 
``` 
User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 236a1745-0896-4be1-9486-7e7f3ab8af19 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive   

```
4. Тело запроса - Request body   

нет   

5. Заголовки ответа - Response headers   
```   
Content-Type: application/json; charset=utf-8; v=1.0 

Date: Fri, 22 Sep 2023 14:01:33 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

api-supported-versions: 1.0 

```     
6. Тело ответа - Response body  
```   

[{"id":1,"title":"Book 1","description":"Dolore consequat sit labore amet elitr diam in magna labore labore. Ipsum et eos dolor kasd sanctus sea velit diam elitr doming sit dolor elitr et dolor. Duo nonumy consectetuer ipsum est labore placerat sed delenit magna at sed dignissim. Nonummy kasd est erat dolores duo facilisis ea.\n","pageCount":100,"excerpt":"Accusam nonumy ut euismod takimata dolor "},... 

```   
## POST/api/v1/Books   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books 

2.	 Ожидаемый результат   

Тело ответа корректное, соответствует POST-запросу на создание новой книги  

HTTP status: 200 - Sucсess   

3.	Заголовки запроса - Request headers   
``` 

Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 59a95c2f-41ec-4ccc-9d3b-28ded92f2978 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 

``` 
4.	Тело запроса - Request body  
``` 
{ 
 "id": 205, 

 "title": "mama", 

 "description": "papa", 

 "pageCount": 1000, 

 "excerpt": "my", 

 "publishDate": "2023-09-20T21:00:52.702Z" 
} 
``` 
5.	Заголовки ответа - Response headers  

```   
Content-Type: application/json; charset=utf-8; v=1.0 

Date: Fri, 22 Sep 2023 18:34:30 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

api-supported-versions: 1.0 
``` 
6.	Тело ответа - Response body    
``` 
{"id":205,"title":"mama","description":"papa","pageCount":1000,"excerpt":"my","publishDate":"2023-09-20T21:00:52.702Z"}   
```   
## POST/api/v1/Books 

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books   

2.	 Ожидаемый результат  

Тело ответа корректное, содержит сообщение о том, что допущена ошибка  

HTTP status: 400 Bad Request 

3.	Заголовки запроса - Request headers   
```
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 689378d6-1106-4561-ba6a-34d94c6e1219 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 

``` 
4.	Тело запроса - Request body   
``` 
{ 
 "id": null, 

 "title": "string", 

 "description": "string", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-20T21:07:26.912Z" 
} 
``` 
5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 18:44:27 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

```   
6.	Тело ответа - Response body    

``` 
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-f3e0453a7c952d4696b174f02dff03e2-de77b03f795c4445-00","errors":{"$.id":["The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 11."]}} 

```   
## POST/api/v1/Books 

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books   

2.	Ожидаемый результат  

Тело ответа корректное, содержит сообщение о недопустимом значении   

HTTP status: 400 Bad Request 

3.	Заголовки запроса - Request headers   

``` 
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 4ae253fb-bb80-4c9c-a1b1-c60c205eee1b 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 

```   
4.	Тело запроса - Request body   
``` 
{ 
 null 

 "excerpt": "string", 

 "publishDate": "2023-09-20T21:36:29.766Z" 
} 
```   
5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 18:51:47 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 
```   
6.	Тело ответа - Response body    
``` 
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-6442445ea9c3f24082086a8ce4b6c880-03650e438b5f3f4b-00","errors":{"$":["'n' is an invalid start of a property name. Expected a '\"'. Path: $ | LineNumber: 1 | BytePositionInLine: 1."]}}   
``` 
## POST/api/v1/Books  

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books   

2.	Ожидаемый результат  

Тело ответа корректное, содержит сообщение о недопустимом значении   

HTTP status: 400 Bad Request 

3.	Заголовки запроса - Request headers   

``` 
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 9b27315a-9cfe-4077-9aaa-a1379a603c0d 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 

```   
4.	Тело запроса - Request body   

``` 
{ 
 "id": 0, 

 "title": , 

 "description": "string", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-20T22:11:07.016Z" 
} 
```   
5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 18:58:24 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

```   
6.	Тело ответа - Response body    

``` 
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-7ec30b78e4d6c84a9b1bc4b3374ad2f9-2065de3b6605dc49-00","errors":{"$.title":["',' is an invalid start of a value. Path: $.title | LineNumber: 2 | BytePositionInLine: 10."]}} 

``` 
## POST/api/v1/Books  

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books   

2.	Ожидаемый результат  

Тело ответа корректное, содержит сообщение об ошибке   

HTTP status: 400 Bad Request 

3.	Заголовки запроса - Request headers   
``` 
User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: fb5ac971-c5b0-46a3-9cf3-39a3314f76fc 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
```  
4.	Тело запроса - Request body   

нет   

5.	Заголовки ответа - Response headers   
``` 
Content-Length: 0 

Date: Fri, 22 Sep 2023 19:03:12 GMT 

Server: Kestrel 
```  
6.	Тело ответа - Response body    
``` 
{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13", 

    "title": "Unsupported Media Type", 

    "status": 415, 

    "traceId": "00-64fff230f00c9a469994eb67dbabb6d1-022ec522b89d4a4e-00" 
} 
```   
## POST/api/v1/Books  

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books   

2.	Ожидаемый результат  

Тело ответа корректное, содержит сообщение, что JSON неверный 

HTTP status: 400 Bad Request 

3.	Заголовки запроса - Request headers   
``` 
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: ae69a973-d1bc-4fa3-a515-b129d2a62515 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
```   
4.	Тело запроса - Request body   
``` 
{ 

 "id": 0, 

 "title": 1, 

 "description": "string", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-22T03:41:57.286Z" 
} 
``` 
5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 19:13:06 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 
```   
6.	Тело ответа - Response body    
``` 
{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1", 

    "title": "One or more validation errors occurred.", 

    "status": 400, 

    "traceId": "00-e9671a2ebe545f4798019c8cd4ce2bf8-db96a60dbeede14d-00", 

    "errors": { 

        "$.title": [ 

            "The JSON value could not be converted to System.String. Path: $.title | LineNumber: 2 | BytePositionInLine: 11." 
        ] 
    } 
} 
``` 
## GET​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/30   

2.	 Ожидаемый результат   

Тело ответа корректное, соответствует GET запросу на получение книги с указанным id  

HTTP status: 200 - Sucсess     

3.	Заголовки запроса - Request headers  
``` 
User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 6fbad10b-4e86-4169-9f0e-29d6b96b90f8 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
```  
4.	Тело запроса - Request body   

нет   

5.	Заголовки ответа - Response headers   
```
Content-Type: application/json; charset=utf-8; v=1.0 

Date: Fri, 22 Sep 2023 19:30:50 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

api-supported-versions: 1.0 
```   
6.	Тело ответа - Response body    
``` 
{ 
    "id": 30, 

    "title": "Book 30", 

    "description": "Stet no dolor labore aliquip sadipscing ea ut dolor molestie autem placerat nostrud amet ut. Ut veniam dolor sit duis nonumy labore consequat accusam kasd ex no magna at facilisis. Accusam voluptua et laoreet duo eos. Rebum esse elitr rebum doming consequat dolor eum assum takimata nonumy no ipsum est accusam te labore. In tempor et sea dolor labore magna justo eirmod ullamcorper eum hendrerit ut vulputate. Illum eos et ea dolor et stet ipsum magna sea. Cum dolores sed id praesent dolores rebum dolores dolor odio ea delenit amet suscipit. Amet nonumy erat lorem justo et nihil dolor. Et commodo no consequat sed gubergren iusto voluptua aliquam sit clita sit clita. Takimata quis ipsum laoreet et dolor dolores sanctus invidunt feugiat dolore. Duo clita assum nonumy justo at dolor vulputate vero et sit. Sit rebum duis. Magna ut autem consequat rebum magna elitr ea sea est dolor enim labore ad vel iriure.\n", 

    "pageCount": 3000, 

    "excerpt": "Vero sanctus consetetur dolore minim sea nulla vulputate sit duis diam sea nobis amet dolor invidunt. Facer eu ipsum et dolore quis tempor voluptua rebum eu molestie dolore duo imperdiet accusam sit sit luptatum. Quod ipsum kasd suscipit et magna sea labore nisl duo diam sed sanctus diam clita. Dolor erat rebum dolor. Sed sit ipsum aliquyam nulla lorem dolore duo diam te. Justo diam nonumy laoreet vero minim feugiat in nam no et id sanctus. Ipsum ipsum suscipit dignissim rebum et hendrerit volutpat at. Labore in vero aliquyam tempor gubergren lorem gubergren lorem imperdiet vero et vel nihil hendrerit dolore aliquyam sanctus feugiat. Dolore esse gubergren et vero ipsum id eirmod accusam clita accumsan soluta autem ipsum tempor labore et ipsum sed.\nUt nonumy dolor no eum gubergren stet sit dolore justo elitr erat kasd quis sed duo. Praesent ea dolore dolore. Ipsum dolor est amet eos eirmod sed justo diam invidunt sanctus ut sed dolore adipiscing tempor. Zzril dolore diam dolor dolore eum ut amet amet nonumy consetetur. Vulputate augue enim sanctus dolor at augue voluptua et clita clita nostrud tempor nulla lorem eirmod eros consequat. Consetetur accusam velit blandit invidunt sit nulla labore ipsum.\nTempor diam ipsum dolor voluptua diam sit stet. Ea duo quod takimata dolore ea ipsum accusam invidunt sit dolor stet ipsum sed voluptua enim. Ut et in sit accusam diam aliquyam praesent sed elitr dolore dignissim at voluptua cum magna eros. Dolore no sit amet justo accusam sit nulla.\nEum dolor tation vero diam dolor elit suscipit ut amet ad. Ipsum clita justo sed diam et amet elitr. Consetetur at ipsum amet diam sit et eirmod diam ad. At elitr magna justo vero sed no eum ut erat illum ipsum ipsum nulla sea. Sit dolore et vulputate no no ipsum vero et justo et amet ad et. Ut aliquam et. Diam volutpat erat sit magna in voluptua justo sed invidunt aliquyam. Nonumy sed consetetur magna congue lorem clita nonumy erat mazim elitr kasd ipsum et labore consetetur ea nam. Odio commodo consequat qui quis justo sadipscing sed. Aliquyam sea accusam nobis vel amet ipsum gubergren consequat voluptua nobis velit diam duo erat. Sanctus justo ipsum. Option illum dolor aliquam sit. Eos et magna placerat autem clita ut. Accusam tincidunt veniam labore aliquyam possim sit dolor amet labore eirmod. Labore aliquyam ut et invidunt. Ea elitr ut laoreet. Labore dolor no dolore labore feugait et eos illum ea tempor in dolores.\nUt odio no nulla eirmod. Erat et duo ipsum augue laoreet nam dolor sed amet aliquyam et nostrud esse lorem dolor kasd. Amet sed aliquam. Invidunt sit sanctus dolores duo ipsum illum ipsum hendrerit sit vero lobortis. Est velit imperdiet duo. Ea at est ut. Invidunt nonumy vel feugiat eu sadipscing lorem magna sit eirmod nobis aliquip diam. Gubergren facer suscipit amet dolore aliquam et takimata veniam sit lorem wisi dolore sadipscing sit. Voluptua et sadipscing tempor dolore sit sadipscing eu amet gubergren sed consequat feugait. Hendrerit vero sanctus nulla eu sadipscing eirmod rebum amet blandit. Vero doming stet erat. Dolor sea diam et esse nostrud sanctus nibh ut diam erat justo vel ea eros ex. Justo sit tempor est takimata iusto velit magna ipsum et amet ipsum praesent sit at nonumy accusam. Rebum sed ut dolores magna duis tempor eos elitr tempor nulla veniam est est. Sed aliquyam est facilisis stet at odio et rebum diam tempor. Sit praesent amet illum dolore ea. Sit exerci et suscipit takimata amet assum vulputate placerat sadipscing consetetur stet aliquyam stet diam.\n", 

    "publishDate": "2023-08-23T19:30:27.0028387+00:00" 
} 
``` 
## GET​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/205   

2.	 Ожидаемый результат   

Тело ответа корректное, содержит сообщение о том, что допущена ошибка  

HTTP status: 400 Bad Request     

3.	Заголовки запроса - Request headers  
``` 
User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 6fbad10b-4e86-4169-9f0e-29d6b96b90f8 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
```   
4.	Тело запроса - Request body   

нет   

5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/json; charset=utf-8; v=1.0 

Date: Fri, 22 Sep 2023 19:30:50 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

api-supported-versions: 1.0 
```   
6.	Тело ответа - Response body    
``` 
{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4", 

    "title": "Not Found", 

    "status": 404, 

    "traceId": "00-a38160cd9e7eaf4a98e8f468759547b7-08707d2f8ea9b94e-00" 
} 
``` 
## PUT​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/5 

2.	 Ожидаемый результат   

Тело ответа корректное, соответствует PUT запросу   

HTTP status: 200 - Sucсess   

3.	Заголовки запроса - Request headers   
``` 
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: bfac61ca-2f4f-4a9e-9e1b-674ac5c60ec6 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
``` 
4.	Тело запроса - Request body   
``` 
{ 
 "id": 5, 

 "title": "mama", 

 "description": "papa", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-22T08:12:48.170Z" 
} 
``` 
5.	Заголовки ответа - Response headers  
``` 
Content-Type: application/json; charset=utf-8; v=1.0 

Date: Fri, 22 Sep 2023 19:53:09 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 

api-supported-versions: 1.0 
```   
6.	Тело ответа - Response body    
``` 
{ 
    "id": 5, 

    "title": "mama", 

    "description": "papa", 

    "pageCount": 0, 

    "excerpt": "string", 

    "publishDate": "2023-09-22T08:12:48.17Z" 
} 
```   
## PUT​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/5 

2.	 Ожидаемый результат   

Тело ответа корректное, содержит сообщение о том, что допущена ошибка  

HTTP status: 400 Bad Request   

3.	Заголовки запроса - Request headers   
```
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: a350972f-0818-4326-ad62-27732df71089 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
``` 
4.	Тело запроса - Request body   
``` 
{ 
 "id": yes, 

 "title": "mama", 

 "description": "papa", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-22T08:12:48.170Z" 
} 
``` 
5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 19:58:07 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 
```  
6.	Тело ответа - Response body    
``` 
{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1", 

    "title": "One or more validation errors occurred.", 

    "status": 400, 

    "traceId": "00-0ba126663425b9419c4f4e11b1583e58-a0e972be1ee04a4f-00", 

    "errors": { 

        "$.id": [ 

            "'y' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 7." 
        ] 
    } 
} 
```   
## PUT​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/5 

2.	 Ожидаемый результат   

Тело ответа корректное, содержит сообщение о том, что допущена ошибка  

HTTP status: 400 Bad Request   

3.	Заголовки запроса - Request headers   
``` 
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: 5f3c0b44-e115-4223-8e23-06a4d737ef9a 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
``` 
4.	Тело запроса - Request body   
``` 
{ 
 "id": 0, 

 "title":  

 "description": "string", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-21T21:45:17.413Z" 
} 
``` 
5.	Заголовки ответа - Response headers  
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 20:01:08 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 
```  
6.	Тело ответа - Response body    
``` 
{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1", 

    "title": "One or more validation errors occurred.", 

    "status": 400, 

    "traceId": "00-beb3b32ec292104ca33dd200e66bf583-337170b1311c474b-00", 

    "errors": { 

        "$": [ 

            "':' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 3 | BytePositionInLine: 14." 
        ] 
    } 
} 
```
## PUT​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/5 

2.	 Ожидаемый результат   

Тело ответа корректное, содержит сообщение о том, что запрос некорректен  

HTTP status: 415   

3.	Заголовки запроса - Request headers   

``` 
User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: fb63aebb-a762-4d30-8b61-3946a18ecf3a 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
``` 
4.	Тело запроса - Request body   

нет 

5.	Заголовки ответа - Response headers  
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 20:04:36 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 
```   
6.	Тело ответа - Response body    
``` 
{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13", 

    "title": "Unsupported Media Type", 

    "status": 415, 

    "traceId": "00-1d94cac3a6684748b88c40aea5069f09-269d9ce0ba844b46-00" 
} 
```
## PUT​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/5 

2.	 Ожидаемый результат   

Тело ответа корректное, содержит сообщение об ошибке  

HTTP status: 400   

3.	Заголовки запроса - Request headers   
``` 
Content-Type: application/json 

User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: f92e9eba-253b-4ad7-b3f0-a627d74716b7 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
``` 
4.	Тело запроса - Request body   
``` 
{ 
 "id": 0, 

 "title":1   

 "description": "string", 

 "pageCount": 0, 

 "excerpt": "string", 

 "publishDate": "2023-09-21T21:45:17.413Z" 
} 
```   
5.	Заголовки ответа - Response headers   
``` 
Content-Type: application/problem+json; charset=utf-8 

Date: Fri, 22 Sep 2023 20:10:01 GMT 

Server: Kestrel 

Transfer-Encoding: chunked 
```  
6.	Тело ответа - Response body    
``` 
{{ 
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1", 

    "title": "One or more validation errors occurred.", 

    "status": 400, 

    "traceId": "00-39e3d3c57a917c42a353d440c65f8518-671f81519793e348-00", 

    "errors": { 

        "$.title": [ 

            "The JSON value could not be converted to System.String. Path: $.title | LineNumber: 2 | BytePositionInLine: 10." 
        ] 
    } 
} 
```
## DELETE​/api​/v1​/Books​/{id}   

1.	URL   

https://fakerestapi.azurewebsites.net/api/v1/Books/20   

2.	 Ожидаемый результат   

Тело ответа корректное, соответствует запросу на удаление книги по id  

HTTP status: 200 - Sucсess     

3.	Заголовки запроса - Request headers   
``` 
User-Agent: PostmanRuntime/7.33.0 

Accept: */* 

Cache-Control: no-cache 

Postman-Token: e5830efc-ee1e-48cc-ba99-42c4109bb13e 

Host: fakerestapi.azurewebsites.net 

Accept-Encoding: gzip, deflate, br 

Connection: keep-alive 
```   
4.	Тело запроса - Request body  

нет 

5.	Заголовки ответа - Response headers   
``` 
Content-Length: 0 

Date: Fri, 22 Sep 2023 20:13:40 GMT 

Server: Kestrel 

api-supported-versions: 1.0 
```   
6.	Тело ответа - Response body    

нет 

# CoverPhotos:

## GET/api/v1/CoverPhotos

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Тело ответа корректное, имеет список всех обложек, в котором обозначены id обложки, id книги и URL обложки.

HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 6571fa00-4505-4176-b8b4-8d58ecadf446
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 09:00:17 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
[
    {
        "id": 1,
        "idBook": 1,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
    },
    {
        "id": 2,
        "idBook": 2,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
    },
...
]
```
## GET/api​/v1​/CoverPhotos​/books​/covers​/1

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/1

2. Тело ответа корректное, соответствует GET запросу на получение информации об обложке определенной книги c id=1 и обозначен url обложки

HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 1516ebf7-752f-4b10-bb80-6103c35c11ec
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 09:28:15 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
[
  {
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  }
]
```
## GET/api​/v1​/CoverPhotos​/books​/covers​/10000000000 - Error 

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/10000000000

2. Тело ответа корректное, соответствует GET запросу на получение информации о обложке определенный книги с id=10000000000 , которая отсутствует в каталоге 

HTTP status: 400 - Bad Request

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: bd1cb36b-5b06-4a24-9588-7c19c52b1afc
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 09:37:53 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e2c083561d55cd42a58f1501bcb03539-6690371b31418d46-00",
  "errors": {
    "idBook": [
      "The value '10000000000' is not valid."
    ]
  }
}
```
## GET/api/v1/CoverPhotos/1

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1

2. Тело ответа корректное, соответствует GET запросу на получение информации об обложке id=1 и обозначен ее url

HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: bce8a9fe-0702-4cd2-a317-e4c9d319befa
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 09:45:10 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
}
```
## GET/api/v1/CoverPhotos/10000000000 - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/10000000000

2. Тело ответа корректное, соответствует GET запросу на получение информации о обложке с id=10000000000 , которая отсутствует в каталоге 

HTTP status: 400 - Bad Request

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 73c44896-1eae-4464-a7f9-ede73f8706fd
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 09:52:15 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-899acadc76742744a474cf6fc1645ef5-b187df33f5aee849-00",
    "errors": {
        "id": [
            "The value '10000000000' is not valid."
        ]
    }
}
```
## POST/api/v1/CoverPhotos

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Тело ответа корректное, соответствует POST запросу на добавление обложки id=1

HTTP status: 200 - Sucсess

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 8b05c21b-88d3-41c5-9e93-4aeb7aae5579
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
  "idBook": 1,
  "url": "string"
}
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 10:39:56 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
{
    "id": 1,
    "idBook": 1,
    "url": "string"
}
```
## POST/api/v1/CoverPhotos - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 7d6c4a9e-7d98-4bac-be7a-a2e9babf4827
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 10:42:38 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3d1c509647dd3945ae069c77f42a5325-1cc7ba1593220a47-00",
    "errors": {
        "$": [
            "The JSON object contains a trailing comma at the end which is not supported in this mode. Change the reader options. Path: $ | LineNumber: 2 | BytePositionInLine: 0."
        ]
    }
}
```
## POST/api/v1/CoverPhotos - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 415 Unsupported Media Type

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: ee4a1604-5ed9-417c-9f24-265b227e9b4c
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 10:49:10 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title": "Unsupported Media Type",
    "status": 415,
    "traceId": "00-3c7b3ace2d3225488c0528005984f345-d8636ff6585b1a41-00"
}
```
## POST/api/v1/CoverPhotos - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 9ea9c867-52d6-45f4-acfc-7d75b8fc9947
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": foreveryoung,
  "idBook": 0,
  "url": "string"
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 10:51:59 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-cb1b6217585a3640a9f870d9ab92a524-bce626fd9d592542-00",
    "errors": {
        "$.id": [
            "'foreveryoung,\r\n  \"idBook\": 0,\r\n  \"url\": \"string\"\r\n}' is an invalid JSON literal. Expected the literal 'false'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
        ]
    }
}
```
## PUT/api/v1/CoverPhotos/1

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1

2. Тело ответа корректное, соответствует PUT запросу на изменение информации об обложке id=1

HTTP status: 200 - Sucсess

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 607b918a-cdbd-49ee-a07f-0506d333eb20
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
  "idBook": 1,
  "url": "string"
}
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 18:03:34 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
{
    "id": 1,
    "idBook": 1,
    "url": "string"
}
```
## PUT/api/v1/CoverPhotos/1 - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c2bc04de-bf13-4f6b-be6c-69d246be1427
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:08:02 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-ae4ddffdda0eff40a7adf4c75f452fa8-e757b65858f8914a-00",
    "errors": {
        "$": [
            "The JSON object contains a trailing comma at the end which is not supported in this mode. Change the reader options. Path: $ | LineNumber: 2 | BytePositionInLine: 0."
        ]
    }
}
```
## PUT/api/v1/CoverPhotos/{id} - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 415 Unsupported Media Type

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 81599d24-4f0e-45ea-bce9-d2650e1eeb49
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:10:16 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title": "Unsupported Media Type",
    "status": 415,
    "traceId": "00-abf59189a781bb4c838fd90de4c13378-693a77090491e240-00"
}
```
## PUT/api/v1/CoverPhotos/foreveryoung - Error

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 89903330-2f1f-40b0-88eb-2450e5b4aaae
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": foreveryoung,
  "idBook": 0,
  "url": "string"
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:12:30 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-ad45c9c942abdc408811c81fc81f89cb-b73339c2eebdc247-00",
    "errors": {
        "$.id": [
            "'foreveryoung,\r\n  \"idBook\": 0,\r\n  \"url\": \"string\"\r\n}' is an invalid JSON literal. Expected the literal 'false'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
        ]
    }
}
```
## DELETE/api/v1/CoverPhotos/1

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1

2. HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 577c9518-ebc3-431c-b5b2-2441029f3284
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Length: 0
Date: Wed, 20 Sep 2023 18:15:50 GMT
Server: Kestrel
api-supported-versions: 1.0
```
6. Response body - Нет

# Users: 

## GET/api/v1/Users

1. https://fakerestapi.azurewebsites.net/api/v1/Users

2. Тело ответа имеет список всех пользователей, где обозначены id, Username и Password пользователя

HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b81a5cc6-0d40-4745-b2c6-ce6a1aeaeb4d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 18:18:27 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
[
    {
        "id": 1,
        "userName": "User 1",
        "password": "Password1"
    },
    {
        "id": 2,
        "userName": "User 2",
        "password": "Password2"
    },
...
]
```
## GET/api/v1/Users/1

1. https://fakerestapi.azurewebsites.net/api/v1/Users/1

2. Тело ответа корректное, соответствует GET запросу на получение информации об пользователе id=1 и обозначен его url

HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 55ed9dda-0c22-4f52-a0f6-e42c83d1ecd5
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 18:21:32 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
{
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
}
```
## GET/api/v1/Users/10000000000 - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users/10000000000

2. Тело ответа корректное, соответствует GET запросу на получение информации о пользователе с id=10000000000 , который отсутствует в каталоге 

HTTP status: 400 - Bad Request

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 9fd42b1f-0d28-4e1b-8429-8d56335fafd0
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:25:57 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3f7cff8464eea748aa9caaeec0d512cf-5a1d9ad33541eb4a-00",
    "errors": {
        "id": [
            "The value '10000000000' is not valid."
        ]
    }
}
```
## POST/api/v1/Users

1. https://fakerestapi.azurewebsites.net/api/v1/Users

2. Тело ответа корректное, соответствует POST запросу на добавление пользователя

HTTP status: 200 - Sucсess

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: ef9e0641-c255-4410-9a7a-92b9810bd9fe
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
  "userName": "string",
  "password": "string"
}
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 18:28:15 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
{
    "id": 1,
    "userName": "string",
    "password": "string"
}
```
## POST/api/v1/Users - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c911ffd3-d9d7-4a2a-9baa-81623940d3fd
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:31:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-5e8f1f41c064e34d9bc54dd6223c2d51-22066695db24744b-00",
    "errors": {
        "$": [
            "The JSON object contains a trailing comma at the end which is not supported in this mode. Change the reader options. Path: $ | LineNumber: 2 | BytePositionInLine: 0."
        ]
    }
}
```
## POST/api/v1/Users - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 415 Unsupported Media Type

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 7772f712-a943-45b1-84ee-35a279766185
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:37:34 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title": "Unsupported Media Type",
    "status": 415,
    "traceId": "00-a51f52e8bb05dd448c08c156fb52bf56-bea1af122842764f-00"
}
```
## POST/api/v1/Users - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 5f5951ce-29e8-4f9a-8f5b-f9d90639d24d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": foreveryoung,
  "userName": "string",
  "password": "string"
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:40:01 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-27d2be53b3269245aa8650ddbb46487a-059a8b45a28dcc4d-00",
    "errors": {
        "$.id": [
            "'foreveryoung,\r\n  \"userName\": \"string\",\r\n  \"password\": \"string\"\r\n}' is an invalid JSON literal. Expected the literal 'false'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
        ]
    }
}
```
## PUT /api/v1/Users/1

1. https://fakerestapi.azurewebsites.net/api/v1/Users/1

2. Тело ответа корректное, соответствует PUT запросу на изменение информации об пользователе с id=1 

HTTP status: 200 - Sucсess

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b91b0afc-4ceb-464d-a07b-bb0e91bf8632
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
  "userName": "string",
  "password": "string"
}
```
5. Response headers
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 20 Sep 2023 18:43:08 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Response body
```
{
    "id": 1,
    "userName": "string",
    "password": "string"
}
```
## PUT /api/v1/Users/1 - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users/1

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 6cd23111-4b7a-4578-8a38-0e3f58a5695d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": 1,
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:45:41 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-7b58f18178826c4aaf86607219eabff5-a94c3d0d48702246-00",
    "errors": {
        "$": [
            "The JSON object contains a trailing comma at the end which is not supported in this mode. Change the reader options. Path: $ | LineNumber: 2 | BytePositionInLine: 0."
        ]
    }
}
```
## PUT /api/v1/Users/1 - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users/1

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 415 Unsupported Media Type

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: d8c186a0-e83e-46d7-8b1b-9b6cb40072a8
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:47:37 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.13",
    "title": "Unsupported Media Type",
    "status": 415,
    "traceId": "00-c1fe27d4a99881449d95134afe49eb4e-1824b1452451bc4c-00"
}
```
## PUT /api/v1/Users/{id} - Error

1. https://fakerestapi.azurewebsites.net/api/v1/Users/1

2. Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status: 400 Bad Request

3. Request headers
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 5200a8c6-1e27-4ab3-b1c0-32196198d8f6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body
```
{
  "id": foreveryoung,
  "userName": "string",
  "password": "string"
}
```
5. Response headers
```
Content-Type: application/problem+json; charset=utf-8
Date: Wed, 20 Sep 2023 18:50:11 GMT
Server: Kestrel
Transfer-Encoding: chunked
```
6. Response body
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-128782da4281c643a1d273a79a01a0bb-45b92adcd410d041-00",
    "errors": {
        "$.id": [
            "'foreveryoung,\r\n  \"userName\": \"string\",\r\n  \"password\": \"string\"\r\n}' is an invalid JSON literal. Expected the literal 'false'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
        ]
    }
}
```
## DELETE /api/v1/Users/1

1. https://fakerestapi.azurewebsites.net/api/v1/Users/1

2. HTTP status: 200 - Sucсess

3. Request headers
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 9305ddb5-d1b1-46be-b460-a9e5b43c591d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Request body - Нет

5. Response headers
```
Content-Length: 0
Date: Wed, 20 Sep 2023 18:52:21 GMT
Server: Kestrel
api-supported-versions: 1.0
```
6. Response body - Нет

