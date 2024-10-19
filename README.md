# North Pole Security Protos

This repository contains protobuf definitions used by Santa.

It also contains generated Go code for these protos, so that the protos can be
imported by projects that don't use Bazel as their build system. There is a
GitHub actions workflow that will automatically re-generate the Go code upon
push/pull request.

If it would be helpful to have BUILD rules or pre-generated files for other
languages, please open an Issue.
