# gqltool

gqlgen.yml:
```yaml
...
models:
  ID:
    model:
      - github.com/99designs/gqlgen/graphql.ID
      - github.com/99designs/gqlgen/graphql.Int
      - github.com/99designs/gqlgen/graphql.Int64
      - github.com/99designs/gqlgen/graphql.Int32
  Int:
    model:
      - github.com/99designs/gqlgen/graphql.Int
      - github.com/99designs/gqlgen/graphql.Int64
      - github.com/99designs/gqlgen/graphql.Int32
  Timestamp:
    model:
      - github.com/husamettinarabaci/gqltool/timestamp.Timestamp
```

*.graphql:
```graphql
type <Your Class> {
  ...
  DateField: Timestamp!
  ...
}
```

```go
go get -u github.com/husamettinarabaci/gqltool
```