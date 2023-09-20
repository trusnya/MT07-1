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
  
Тело ответа корректное, соответствует GET запросу на изменение информации об активности с id 5   

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

HTTP status: 400Bad Request

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

HTTP status: 400Bad Request

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
5.Заголовки ответа
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

2. 

3. Request headers
```

```
4. Request body
```

```
5. Response headers
```

```
6. Response body
```

```
## PUT/api/v1/CoverPhotos/{id}

## DELETE/api/v1/CoverPhotos/{id}

# Users: 

## GET/api/v1/Users

## GET/api/v1/Users/{id}

## POST/api/v1/Users

## PUT /api/v1/Users/{id}

## DELETE /api/v1/Users/{id}