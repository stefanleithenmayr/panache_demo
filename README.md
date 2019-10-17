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
curl -d '{"name": "Stefan Leithenmayr"}' -H "Content-Type: application/json" -X POST http://localhost:8080/student
```
