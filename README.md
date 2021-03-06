# GoogleLanguageService

[![Build Status](https://travis-ci.com/sivakon/grpc-julia-gcp-example.svg?branch=master)](https://travis-ci.com/sivakon/grpc-julia-gcp-example)

## __Except `GoogleLanguageService.jl` everything is autogenerated.__

Added TravisCI

Generate ProtoBuf stubs.
> These ProtoBuf files are just binary representation of data with a specified schema.

This repository is direct translation of [Swift Example](https://github.com/googleapis/googleapis.github.io/blob/master/examples/rpc/swift/SETUP.sh)

```
protoc google/cloud/language/v1/language_service.proto \
  google/api/annotations.proto google/api/http.proto \
  -Igoogleapis \
  --julia_out=GoogleLanguageService/src/
```

## Julia inspiration taken from Protobuf example
https://github.com/JuliaIO/ProtoBuf.jl/blob/master/test/services/testsvc.jl

## API should be like this
https://github.com/googleapis/google-cloud-python/blob/master/language/samples/v1/language_entity_sentiment_gcs.py

## What's happening
- We HTTP POST to the API endpoint (protobuf byte stream) and receiving in the same format

## Julia HTTP
https://juliaweb.github.io/HTTP.jl/stable/
