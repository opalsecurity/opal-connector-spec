# How to generate an OpenAPI connector

## Prerequisites

### Install OpenAPI Generator

```
brew install openapi-generator
```

### Generating the server stub

Check [OpenAPI Generator documentation](https://openapi-generator.tech/docs/generators/#server-generators)
for available server generators.

Clone this repository, then proceed by generating the connector server stub.
Check available configuration options for your chosen server generator to tweak
the output of the generated code.

```
git clone https://github.com/opalsecurity/opal-connector-spec.git
openapi-generator generate -g go-gin-server -i opal-connector-spec/openapi-connector-spec.yaml -o opal-myconnector-connector
```

Replace `go-gin-server` with the preferred server generator.
