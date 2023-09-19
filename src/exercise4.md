# Пример: 
1. URL (вставляйте его прямо со скобками, например, "https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id}}")
2. Ожидаемый результат (своими словами)
3. Заголовки запроса - Request headers (можно посмотреть через консоль в левом нижнем углу)
4. Тело запроса - Request body (если тело слишком большое, то только его часть)
5. Заголовки ответа - Response headers
6. Тело ответа - Response body (если тело слишком большое, то только его часть)

# CoverPhotos:

## GET/api/v1/CoverPhotos

1. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Тело ответа корректное, имеет список всех обложек, в котором обозначены id обложки, id книги и URL обложки.

3. 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 6571fa00-4505-4176-b8b4-8d58ecadf446
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. 

## GET/api​/v1​/CoverPhotos​/books​/covers​/{idBook}

## GET/api/v1/CoverPhotos/{id}

## POST/api/v1/CoverPhotos

## PUT/api/v1/CoverPhotos/{id}

## DELETE/api/v1/CoverPhotos/{id}

# Users: 

## GET/api/v1/Users

## GET/api/v1/Users/{id}

## POST/api/v1/Users

## PUT /api/v1/Users/{id}

## DELETE /api/v1/Users/{id}
