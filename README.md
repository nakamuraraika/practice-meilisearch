# practice-meilisearch

# Run

```sh
docker compose up
curl https://www.meilisearch.com/movies.json -O
curl \
  -X POST 'http://localhost:7700/indexes/movies/documents?primaryKey=id' \
  -H 'Content-Type: application/json' \
  --data-binary @movies.json
```

open http://localhost:7700