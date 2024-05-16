
To generate the docs:

```
npm install -g @adobe/jsonschema2md

# show usage information
jsonschema2md

# run task
jsonschema2md -d schema -o docs/schema
# generated output for whole folder is written to ./docs/schema
```

OR

```
pip install json-schema-for-humans

generate-schema-doc --config description_is_markdown=true --config show_toc=true --config template_name=md ./schema ./docs/md
# generated output for whole folder is written to ./docs/md

generate-schema-doc --config-file jsfh-conf.yaml ./schema ./docs/html
# generated output for whole folder is written to ./docs/html

```


https://o19s.github.io/blob/main/docs/html/event.request.schema.html
