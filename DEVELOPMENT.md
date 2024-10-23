
#### To generate the docs:


```
pip install json-schema-for-humans

export UBI_VERSION=1.2.0

mkdir docs/html/${UBI_VERSION}
/Users/epugh/.asdf/installs/python/3.9.17/bin/generate-schema-doc --config-file jsfh-conf.yaml ./schema/$UBI_VERSION/ ./docs/html/$UBI_VERSION
# generated html for whole folder is written to ./docs/html

```

We then check them into Github.
https://o19s.github.io/blob/main/docs/


#### To release UBI

1. Make sure to copy the last version (i.e. `schema/1.2.0)` to the next version (i.e. `schema/1.3.0`)
1. Make sure to update the version information in each .json file.
1. Build the docs into ./docs/html/1.3.0
1. Update the home README.md file to point to the new version.
