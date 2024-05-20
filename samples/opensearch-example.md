## OpenSearch Example

This assumes you have checked out https://github.com/o19s/chorus-opensearch-edition/ and run the `quickstart.sh` script.

Issue a Query that is to be tracked via UBI:
  
```
curl -X POST -H 'Content-type:application/json' -d '{
  "query": {
    "match": {
      "name": "toner"
    }
  },
  "ext": {
    "ubi": {
      "query_id": "12300d16cb-b6f1-4012-93ebcc49cac90426",
      "user_query": "toner"
    }
  }
}' "http://localhost:9200/ecommerce/_search"
```

__Eventually the `user_query` should take not just a string but a map of all the fields.
