# Read Me First
This project highlights the problem with trying to use the oneOf keyword available in OpenAPI and generate Java code.

## Producing the error
A simple "mvn clean install" executed in the root of this project should produce a build error. The following is the output from a maven build:

    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[30,37] cannot find symbol
    [ERROR]   symbol:   class OneOfCatDog
    [ERROR]   location: package org.openapitools.client.model
    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[31,37] cannot find symbol
    [ERROR]   symbol:   class UNKNOWN_BASE_TYPE
    [ERROR]   location: package org.openapitools.client.model
    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[70,39] cannot find symbol
    [ERROR]   symbol:   class UNKNOWN_BASE_TYPE
    [ERROR]   location: class org.openapitools.client.api.DefaultApi
    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[101,54] cannot find symbol
    [ERROR]   symbol:   class UNKNOWN_BASE_TYPE
    [ERROR]   location: class org.openapitools.client.api.DefaultApi
    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[120,27] cannot find symbol
    [ERROR]   symbol:   class UNKNOWN_BASE_TYPE
    [ERROR]   location: class org.openapitools.client.api.DefaultApi
    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[136,52] cannot find symbol
    [ERROR]   symbol:   class UNKNOWN_BASE_TYPE
    [ERROR]   location: class org.openapitools.client.api.DefaultApi
    [ERROR] /home/aaron/code/openapi-issue/target/generated-sources/openapi/src/gen/java/main/org/openapitools/client/api/DefaultApi.java:[154,40] cannot find symbol
    [ERROR]   symbol:   class UNKNOWN_BASE_TYPE
    [ERROR]   location: class org.openapitools.client.api.DefaultApi

## Expected results
The project should build without errors.
