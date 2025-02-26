
#### To generate the docs:


Generated html for the specific schema is written to `./docs/html/${UBI_VERSION}`.

```
pip install json-schema-for-humans

export UBI_VERSION=1.2.0

mkdir docs/html/${UBI_VERSION}
/Users/epugh/.asdf/installs/python/3.9.17/bin/generate-schema-doc --config-file jsfh-conf.yaml ./schema/$UBI_VERSION/ ./docs/html/$UBI_VERSION

```

We then check them into Github.


#### To release UBI

1. Make sure to copy the last version (i.e. `schema/1.2.0)` to the next version (i.e. `schema/1.3.0`)
1. Make sure to update the version information in each .json file.
1. Build the docs into ./docs/html/1.3.0
1. Update the virtual link to the latest version: 
  1. `ln -s docs/html/1.3.0 docs/html/latest`
  1. `ln -s docs/schema/1.3.0 docs/schema/latest`
1. Check in and merge the changes to the main branch.
1. Create a release on Github.
1. Post on Relevance Slack #user-behavior-insights channel.
1. Update the ubisearch.dev site via https://github.com/o19s/ubi-website
