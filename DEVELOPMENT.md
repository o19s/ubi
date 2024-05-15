
To generate the docs:

```
npm install -g @adobe/jsonschema2md

# show usage information
jsonschema2md

# run task
jsonschema2md -d schemas -o docs/schema
# generated output for whole folder is written to ./docs/schema
```

OR

```
pip install json-schema-for-humans

generate-schema-doc --config description_is_markdown=true --config show_toc=true --config template_name=md ./schema ./docs/md
```
