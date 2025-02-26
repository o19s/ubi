
#### To generate the docs:

We use the Pythong library `json-schema-for-humans` to generate HTML docs based on the JSON schema files.

You need Python to generate the HTML docs. The best way is to use a virtual environment.

As a result the generated HTML for the specific schema is written to `./docs/html/${UBI_VERSION}`.

1. Create a virtual environment

```
python3 -m venv .
```

2. Activate virtual environment

```
source bin/activate
```

3. Install Python lib `json-schema-for-humans`
```
python3 -m pip install json-schema-for-humans
```

4. Export version variable with the corresponding version

```
export UBI_VERSION=1.4.0
```

5. Create folder 

```
mkdir docs/html/${UBI_VERSION}
```

6. Generate docs

```
generate-schema-doc --config-file jsfh-conf.yaml ./schema/$UBI_VERSION/ ./docs/html/$UBI_VERSION
```

We then check them into Github.

#### To release UBI

1. Make sure to copy the last version (i.e. `schema/1.2.0)` to the next version (i.e. `schema/1.3.0`)
1. Make sure to update the version information in each `.json` file.
1. Build the docs into `./docs/html/1.3.0` (see steps above)
1. Update the virtual link to the latest version: 
  1. `ln -s docs/html/1.3.0 docs/html/latest`
  1. `ln -s docs/schema/1.3.0 docs/schema/latest`
1. Check in and merge the changes to the main branch.
1. Create a release on Github.
1. Post on Relevance Slack #user-behavior-insights channel.
1. Update the ubisearch.dev site via https://github.com/o19s/ubi-website
