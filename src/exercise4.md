# Пример: 

1. URL (вставляйте его прямо со скобками, например, "https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id}}")
2. Ожидаемый результат (своими словами) + HTTPS status
3. Заголовки запроса - Request headers (можно посмотреть через консоль в левом нижнем углу)
4. Тело запроса - Request body (если тело слишком большое, то только его часть)
5. Заголовки ответа - Response headers
6. Тело ответа - Response body (если тело слишком большое, то только его часть)

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

2.Ожидаемый результат 
  
Тело ответа корректное, содержит сообщение о том, что допущена ошибка 

HTTP status:415 Unsupported Media Type

3.Заголовки запроса 
  
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
4.Тело запроса 
```
```  
5.Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Tue, 19 Sep 2023 09:56:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6.Тело ответа 
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

(https://fakerestapi.azurewebsites.net/api/v1/Activities/5)

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


# Authors

## GET/api​/v1​/Authors

1. https://fakerestapi.azurewebsites.net/api/v1/Authors

2. HTTP status: 200 - Sucсess

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
```
[
    {
        "id": 1,
        "idBook": 1,
        "firstName": "First Name 1",
        "lastName": "Last Name 1"
    },
    ...
]
```

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

2. HTTP status: 200 - Sucсess

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

2. HTTP status: 400 Error: Bad Request

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

2. HTTP status: 200 - Sucсess

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

2. HTTP status: 400 Error Bad Request

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

2. HTTP status: 200 - Sucсess

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

2. HTTP status: 400 Error Bad Request

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

2. HTTP status: 415 Unsupported Media Type

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

2. HTTP status: 400 Error Bad Request

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

2. HTTP status: 200 - Sucсess

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

2. HTTP status: 400 Error Bad Request

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

2. HTTP status: 415 Unsupported Media Type

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

2. HTTP status: 400 Error Bad Request

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

2. HTTP status: 200 - Sucсess

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
