## Solr Example

Assuming you have started Solr via `bin/solr start -c -e techproducts`.

Create the UBI component:

```
curl -X POST -H 'Content-type:application/json' -d '{
  "add-searchcomponent": {
    "name": "ubi",
    "class": "solr.UBIComponent",
    "defaults":{ }
  }
}' "http://localhost:8983/api/collections/techproducts/config"
``` 

Configure Solr to use the UBI component as part of search requests:

```
curl -X POST -H 'Content-type:application/json' -d '{
  "update-requesthandler": {
    "name": "/select",
    "class": "solr.SearchHandler",
    "last-components":["ubi"]
  }
}' "http://localhost:8983/api/collections/techproducts/config"
```

Issue a Query using Solr's JSON Query format with embedded UBI settings:
  

```
curl -X POST -H 'Content-type:application/json' -d '{
  "query" : "ram OR memory",
  "filter": [
      "inStock:true"
  ],
  "limit":2,
  "params": {
    "ubi": "true",
    "query_id": "xyz890",
    "user_query": "RAM memory",
    "query_attributes": {
      "experiment": "supersecret",      
      "page": 1,
      "filter": "productStatus:available"
    }            
  }
}' "http://localhost:8983/solr/techproducts/select"
```
