# 用Gin框架的GraphQL Demo

Golang Gin + GrapgQL + MongoDB

## Tech

- [Gin](https://github.com/gin-gonic/gin) - Web framework written in Go
- [gqlgen](github.com/99designs/gqlgen) - GraphQL for Go
- [MongoDB](https://github.com/mongodb/mongo-go-driver) - MongoDB Driver API for Go

## Query & Mutation Operation Sample

```sh
mutation {
  createDog(input: {name: "Reo", age: 10}) {
    _id
    name
    age
  }
}

query{
 dog(_id:"hex_id"){name}
}

query{
 dogs{name,age}
}
```
