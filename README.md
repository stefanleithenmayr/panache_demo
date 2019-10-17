# Panache (ORM) - Quarkus

```
docker run --name some-postgres -p 5432:5432 -e POSTGRES_PASSWORD=passme -d postgres
```

application.properties:
```
quarkus.datasource.url = jdbc:postgresql://localhost:5432/postgres
quarkus.datasource.driver = org.postgresql.Driver
quarkus.datasource.username = postgres
quarkus.datasource.password = passme
quarkus.hibernate-orm.database.generation = drop-and-create

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
