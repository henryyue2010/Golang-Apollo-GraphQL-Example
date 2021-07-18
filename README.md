# Golang-Apollo-GraphQL-Example

This is an example of Apollo Federation in Golang to compose multiple GraphQL services into a unified data graph based on microservice architecture.

#### Gateway:

http://localhost:4000


#### User Servce:

http://localhost:4001


#### Profile Service:

http://localhost:4002



### Queries to Gateway:

1.
```
query{
  user{
  id
  name
  }
}
```

2.
```
query{
  user{
    id
    name
    profile{
      userId
      age
      phone
      job
    }
  }
}
```
