<div align="center">

# User Behavior Insights

UBI (or User Behavior Insights) is a(nother) naive attempt to create **a standard open source format to define and share user event tracking information**. The format is defined as a JSON Schema to validate queries and events defined as JSON files.
 
 <a href='https://github.com/o19s/ubi/releases'>
  <img src='https://img.shields.io/github/v/release/o19s/ubi?color=%23FDD835&label=version&style=for-the-badge&logo=JSON' alt="Version Badge">
</a>
<br />
<br />
 
[Why use it](#-why-use-it) •
[How to use it](#-how-to-use-it) •
[Who uses it](#-who-uses-it) •
[Who we are](#-who-we-are) •
[How to contribute](#%EF%B8%8F-how-to-contribute) •
[License](#%EF%B8%8F-license) •
[Spread the word!](#-spread-the-word)  
<br />
<br />
<br />
!["JSON Schema"](https://github.com/o19s/ubi/blob/master/assets/readme/schema_screen_capture.png?raw=true "JSON Schema")
<br />
 <br />
!["UBI Sample"](https://github.com/o19s/ubi/blob/master/assets/readme/MAC_sample.gif?raw=true "MAC Sample")
  
</div>  

## 🥘 Why use it

Many Search teams struggle with understanding "Why is my user doing this".  They have great understanding of an incoming query and the documents returned, but no ability to connect that dot with an indicator of success, such as a click through event or event a add to cart.

There are A LOT of tools out there for tracking events, Google Analytics, Snowplow, etc, but each is a bit different, and each tends to lock you in.  None of them think about the needs of Search teams specifically either.

The User Behavior Insights standard attempts to provide a search focused standard that can operate across many platforms.


<div align="center">
  <img src='https://github.com/o19s/ubi/blob/master/assets/readme/MAC_Structure.png?raw=true' width='600px' alt="UBI Structure">
 </div>


## 🪛 How to use it

The UBI standard is implemented by various platforms, and click through to learn more about using it with your chosen solution.
 * OpenSearch
 * [Apache Solr](https://github.com/apache/solr/pull/2452)
 
UBI requires coordination between the client (a browser, a mobile app, etc) and the backend, which is documented using JSON Schema.  To validate 
You just need to copy, download or reference [the schema](https://github.com/o19s/ubi/blob/master/schema/schema.json) to validate an event, built as a JSON file from scratch, or a JSON generated previously (for example, [this sample](https://github.com/o19s/ubi/blob/master/samples/default_sample_ES.json)).  ** ERIC, what about query versus event **

To get started, you can copy both schema and sample in an **online validator** like [jsonschemavalidator.net](https://www.jsonschemavalidator.net/) or [liquid-technologies.com/online-json-schema-validator](https://www.liquid-technologies.com/online-json-schema-validator).

!["JSON Schema"](https://github.com/o19s/ubi/blob/master/assets/readme/MAC_online_validator_example.png?raw=true "JSON Schema")

You also have implementations to validate a JSON file programmatically in almost every coding language:

* [AVJ (JavaScript)](https://ajv.js.org/)
* [Snow (Java)](https://github.com/ssilverman/snowy-json)
* [jschon (Python)](https://jschon.readthedocs.io/en/latest/)
* ... and [much more](https://json-schema.org/implementations.html)

> :warning: **The current MAC Schema has been designed using the 2019-09 Specification Draft**: When choosing a validator, please, check if it's compliant with the 2019-09 Draft. You can get much more information about the JSON Schema Specification in [json-schema.org](https://json-schema.org/).

You can check **examples of how to use code to create and validate MAC files** in the [MAC/scripts](https://github.com/getmanfred/mac/tree/master/scripts) directory.

---

The Schema is documented by itself, but it's much easier to get "the big picture" with [a graphical representation](https://github.com/getmanfred/mac/blob/master/assets/readme/MAC_diagram.png).
<br />
<br />

## 🎨 Who uses it

We are just trialing using UBI as an interchangeable format **to simplify their understanding of what their users are doing** and are looking for more collaborators.

<a href="https://www.getmanfred.com/" target="_blank"><img alt="Manfred" src="./assets/readme/manfred_logo.jpg?raw=true" width="160"/></a> <a href="https://www.sngular.com/" target="_blank"><img alt="SNGULAR" src="./assets/readme/sngular_logo.png?raw=true" width="160"/></a> <a href="https://mobivery.com/" target="_blank"><img alt="MOBIVERY" src="./assets/readme/mobivery_logo.png?raw=true" width="160"/></a> <a href="https://spartacommodities.com/" target="_blank"><img alt="SPARTA" src="./assets/readme/sparta_logo.png?raw=true" width="160"/></a> <a href="https://www.tinybird.co/" target="_blank"><img alt="TINYBIRD" src="./assets/readme/tinybird_logo.jpg?raw=true" width="160"/></a>

## 🤓 Who we are

As common in new projects, the individual or group who started the project also administers the project, establishes its vision, and controls permissions to merge code into it. **We are thinking about how to establish a more robust governance structure**.

## ⚙️ How to contribute

UBI is an open-source project. We are committed to a fully transparent development process and appreciate highly any contributions. Whether you are helping us fix bugs, proposing new features, improving our documentation or spreading the word - we would love to have you as part of the UBI community.

Please refer to our [Contribution Guidelines](https://github.com/o19s/ubi/blob/master/CONTRIBUTING.md) and [Code of Conduct](https://github.com/o19s/ubi/blob/master/code_of_conduct.md).

## ⚖️ License

UBI is free and open-source software licensed and distributed under the Creative Commons Attribution Share Alike 4.0 International (CC BY-SA 4.0 International). ** ERIC: ASL?? WHat do standards like/  **

## 🌟 Spread the word!

If you want to say thank you and/or support active development of the MAC:

- Add a GitHub Star to the project!
- ???
--?


Thanks so much for your interest in growing the reach of UBI!

_This site was inspired by https://github.com/getmanfred/mac.  Thank you!_
