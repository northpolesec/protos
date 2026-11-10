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

`telemetry/v1.proto` is the schema of the protobuf telemetry that Santa for
macOS writes. See the
[Santa telemetry docs](https://northpole.dev/features/telemetry) for the file
formats.

The telemetry schema is also on BSR. To import it in Go code, add the following
to your imports:

```text
buf.build/gen/go/northpolesec/protos/protocolbuffers/go/telemetry
```
