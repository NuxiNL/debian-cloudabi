# Debian container with CloudABI utilities

This is a container image that is based on Debian testing that includes
a copy of all components of CloudABI. It ships with a cross compiler for
CloudABI (`x86_64-unknown-cloudabi-cc`). It also contains
`cloudabi-run`, the utilty that can be used to run CloudABI
applications.

As Linux does not provide native support for CloudABI, `cloudabi-run`
must be invoked with the `-e` flag to enable userspace system call
emulation.
