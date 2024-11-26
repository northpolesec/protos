# North Pole Security Protos

This repository contains protobuf definitions used by [Santa](https://github.com/northpolesec/santa).

### Buf

The protos are also available at https://buf.build/northpolesec/protos and can
be imported as a dependency into a project using `buf` by adding the following
to the `deps` section of your `buf.yaml`:

```
buf.build/northpolesec/protos
```

You can also import generated proto code directly from buf. For example, to
import the sync proto in Go code add the following to your imports:

```
buf.build/gen/go/northpolesec/protos/protocolbuffers/go/sync
```

