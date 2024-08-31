
To generate the docs:

```
npm install -g @adobe/jsonschema2md

jsonschema2md -d schema -o docs/schema
# generated output for whole folder is written to ./docs/schema
```

OR

```
pip install json-schema-for-humans

/Users/epugh/.asdf/installs/python/3.9.17/bin/generate-schema-doc --config-file jsfh-conf.yaml /Users/epugh/Documents/projects/ubi/schema/1.1.0/ /Users/epugh/Documents/projects/ubi/docs/html/1.1.0
# generated html for whole folder is written to ./docs/html

```

We then check them into Github.


https://o19s.github.io/blob/main/docs/
