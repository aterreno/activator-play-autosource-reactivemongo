```curl -X POST -d '{ "name":"bob", "age":25 }' --header "Content-Type:application/json" http://localhost:9000/persons --include```

```curl -X POST -d '{ "name":"john", "age":43 }' --header "Content-Type:application/json" http://localhost:9000/persons --include```

```curl http://localhost:9000/persons --include```

```curl -X DELETE http://localhost:9000/persons/52f8e8eae68a33c60148138a --include```

```curl -X GET http://localhost:9000/persons/52f8e8eae68a33c60148138a --include```

```curl -X PUT -d '{ "name":"john", "age":35 }' --header "Content-Type:application/json" http://localhost:9000/persons/52f8e8d9e68a33c601481389 --include```

```curl -X POST -d '[{ "name":"johnny", "age":15, "address":{"city":"Paris", "street":"rue quincampoix"} },{ "name":"tom", "age":3, "address":{"city":"Trifouilly", "street":"rue des accidents de poucettes"} }]' --header "Content-Type:application/json" http://localhost:9000/persons/batch --include```

```curl -X POST -d '{"name":{"$regex":"^john"}}' --header "Content-Type:application/json" http://localhost:9000/persons/find --include```

```curl -X DELETE -d '{}' --header "Content-Type:application/json" http://localhost:9000/persons/batch --include```