# goland-demo
Goland Microservice Demo


# Examples


```
$ curl -X GET localhost:8442/
```

```
$ curl -X GET localhost:8442/jump
```

```
$ curl -XPOST -H "Content-type: application/json" -d '{
    "message": "Hello",
    "last_path": "/users",
    "jump_path": "/jump",
    "jumps": [
        "http://localhost:8443",
    ]
}' 'localhost:8442/jump'
```
```
$ curl -XPOST -H "Content-type: application/json" -d '{
    "message": "Hello",
    "last_path": "/jump",
    "jump_path": "/jump",
    "jumps": [
        "http://java-springboot-demo-git:8443",
    ]
}' 'localhost:8442/jump'
```


curl -XPOST -H "Content-type: application/json" -d '{             
    "message": "Hello",
    "last_path": "/jump",
    "jump_path": "/jump",
    "jumps": [
        "http://java-springboot-demo-git:8443"
    ]
}' 'localhost:8442/jump'









curl -XPOST -H "Content-type: application/json" -d '{
    "message": "Hello",
    "last_path": "/jump",
    "jump_path": "/jump",
    "jumps": [
        "http://localhost:8443"
    ]
}' 'localhost:8442/jump'

curl -XPOST -H "Content-type: application/json" -d '{
    "message": "Hello",
    "last_path": "/users",
    "jump_path": "/jump",
    "jumps": [
        "http://localhost:8443"
    ]
}' 'localhost:8442/jump'

curl -XPOST -H "Content-type: application/json" -d '{
    "message": "Hello",
    "last_path": "/jump",
    "jump_path": "/jump",
    "jumps": [
        "http://localhost:8443"
    ]
}' 'localhost:8442/jump'

curl -XGET localhost:8442/jump