# Stress testing

## Tool

`go get -tool github.com/six-ddc/plow@latest`

The request contains a set of validator pubkeys or committee IDs and a range of 150-300 slots.

## endpoint `/v1/exporter/traces/committee`

The response times become unreasonably high when issuing 50 or more parallel requests.

## endpoint `/v1/exporter/traces/validator`

The response times become unreasonably high when issuing 60 or more parallel requests.

## endpoint `/v1/exporter/decideds`

The response times become unreasonably high when issuing 30 or more parallel requests.

Fails to respond if requested 300 slots over 30 parallel requests.
