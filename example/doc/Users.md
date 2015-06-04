## API Documentation
- Table of Contents
  - [GET /api/users?hoge=fuga#aaa=bbb](#user-content-get-apiusershogefugaaaabbb)
  - [GET /api/users/:name](#user-content-get-apiusersname)
  - [POST /api/users](#user-content-post-apiusers)
  - [GET /api/users](#user-content-get-apiusers)
  - [GET /api/users/:name](#user-content-get-apiusersname-1)
  - [POST /api/users](#user-content-post-apiusers-1)

## GET /api/users?hoge=fuga#aaa=bbb

#### Request
```
GET /api/users HTTP/1.1
```

#### Response
```
200
Content-Type: application/json; charset=utf-8

{
  "users" : [ {
    "name" : "Bob",
    "height" : 172
  }, {
    "name" : "Alice",
    "height" : 155
  } ]
}
```

## GET /api/users/:name
find user

#### Request
```
GET /api/users/yuno HTTP/1.1
```

#### Response
```
200
Content-Type: application/json; charset=utf-8

{
  "user" : {
    "name" : "yuno",
    "height" : 163
  }
}
```

## POST /api/users

#### Request
```
POST /api/users HTTP/1.1
X-API-Token: YOUR_API_TOKEN
X-Public-Token: non-secret

{
  "name" : "yuno",
  "height" : 144
}
```

#### Response
```
201
Content-Type: application/json; charset=utf-8

{
  "user" : {
    "name" : "yuno",
    "height" : 144
  }
}
```

## GET /api/users
get all users

#### Request
```
GET /api/users HTTP/1.1
```

#### Response
```
200
Content-Type: application/json; charset=utf-8

{
  "users" : [ {
    "name" : "Bob",
    "height" : 172
  }, {
    "name" : "Alice",
    "height" : 155
  } ]
}
```

## GET /api/users/:name
find user

#### Request
```
GET /api/users/yuno HTTP/1.1
```

#### Response
```
200
Content-Type: application/json; charset=utf-8

{
  "user" : {
    "name" : "yuno",
    "height" : 163
  }
}
```

## POST /api/users

#### Request
```
POST /api/users HTTP/1.1
X-API-Token: YOUR_API_TOKEN
X-Public-Token: non-secret

{
  "name" : "yuno",
  "height" : 144
}
```

#### Response
```
201
Content-Type: application/json; charset=utf-8

{
  "user" : {
    "name" : "yuno",
    "height" : 144
  }
}
```
