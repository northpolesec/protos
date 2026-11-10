# North Pole Security Protos

This repository contains protobuf definitions used by [Santa](https://github.com/northpolesec/santa).

## Buf

The protos are also available at https://buf.build/northpolesec/protos and can
be imported as a dependency into a project using `buf` by adding the following
to the `deps` section of your `buf.yaml`:

```yaml
buf.build/northpolesec/protos
```

You can also import generated proto code directly from buf. For example, to
import the sync proto in Go code add the following to your imports:

```text
buf.build/gen/go/northpolesec/protos/protocolbuffers/go/sync
```

## Telemetry

`telemetry/v1.proto` is the schema of Santa's protobuf telemetry. With the
`EventLogType` `protobuf`, the spool files are a `LogBatch` of `Any`-wrapped
`SantaMessage`. With `protobufstream`, Santa writes length-delimited
`SantaMessage`.

Each Santa release N tags this repository `santa/N` at the schema it was built
with.

The telemetry schema is also on BSR. To import it in Go code, add the following
to your imports:

```text
buf.build/gen/go/northpolesec/protos/protocolbuffers/go/telemetry
```
