# Panache (ORM) - Quarkus

```
docker run --name some-postgres -p 5432:5432 -e POSTGRES_PASSWORD=passme -d postgres
```


JSON - Test
```
{
    "name": "Stefan Leithenmayr"
}
```

Post a Entity:
```
curl -d '{"key1":"value1", "key2":"value2"}' -H "Content-Type: application/json" -X POST http://localhost:3000/data
```
