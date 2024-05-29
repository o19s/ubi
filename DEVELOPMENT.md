
To generate the docs:

```
npm install -g @adobe/jsonschema2md

jsonschema2md -d schema -o docs/schema
# generated output for whole folder is written to ./docs/schema
```

OR

```
pip install json-schema-for-humans

generate-schema-doc --config-file jsfh-conf.yaml ./schema ./docs/html
# generated html for whole folder is written to ./docs/html

```

We then check them into Github.


https://o19s.github.io/blob/main/docs/html/event.request.schema.html
