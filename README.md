### rqlite
---
https://github.com/rqlite/rqlite

```
curl -XPOST 'localhost:4001/db/execute?pretty&timings' -H "Content-Type: application/json" -d '[
  "CREATE TABLE foo (id integer not null primary key, name text)"
]'

curl -G 'localhost:4001/db/query?pretty&timings' --data-urlencode 'q=SELECT * FROM foo'
```

```
{
  "results": [
    {
      "last_insert_id": 1,
      "rows_affected": 1,
      "time": 0.00886
    }
  ],
  "time": 0.0152,
  "raft": {
    "index": 43,
    "node_id": "xxxxxxxxx"
  }
}
```

```
```


