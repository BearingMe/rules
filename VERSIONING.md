# Semantic Versioning

## Summary

Semantic Versioning is a simple set of rules and requirements that dictate how version numbers are assigned and incremented. It’s a way for software authors to communicate succinctly to the consumers of their software important info they should know about this release and also a good tool to keep track of development state internally.

As a standard, the version number must take the form X.Y.Z where none of these are negative integers. X is called the **major** version, Y the **minor**, and Z is the **patch**. Each element must increase numerically. For instance: 1.9.0 -> 1.10.0 -> 1.11.0.

## General Rules

- `Patch` version must be incremented if any new backwards **compatible** bug fix is introduced to the public API
- `Minor` version must be incremented if any new backwards **compatible** functionality is introduced or anyone is  marked as deprecated. Patch version must be reset to 0 when minor version is incremented
- `Major` version must be incremented when any **incompatible** changes are introduced. Patch and minor versions must be reset to * when major version is incremented

Once a versioned package has been released, the contents of that version must not be modified. Any modifications must be released as a new version.

## Early Development

- `Major version zero` (0.y.z) is for initial development. Anything may change at any time. The public API shouldn't be considered stable
- `Version 1.0.0` defines the first stable version of your public API. The way in which the version number is incremented after this release is dependent on this public API and how it changes
- `Pre-release` version may be denoted by appending a hyphen and a series of dot separated identifiers immediately following the patch version. Examples: 1.0.0-alpha, 1.0.0-alpha.1, 1.0.0-0.3.7, 1.0.0-x.7.z.92, 1.0.0-x-y-z.--, etc

## Pre-release

- `Alpha`: This is an early version of the software that is still being developed and may have significant bugs and missing features. Alpha releases are usually not made available to the general public and are intended for internal testing only
- `Beta`: This is a more mature version of the software that has most of its features implemented, but may still have some bugs and issues. Beta releases are often made available to a wider group of users for testing and feedback
- `Release Candidate (RC)`: This is a version of the software that is considered feature-complete and has undergone extensive testing. The purpose of a release candidate is to ensure that the software is stable and ready for production use.

Those rules may not be applied to initial development state

## References

[Semantic Versioning 2.0](https://semver.org/)
[RFC 2119](https://www.rfc-editor.org/rfc/rfc2119)
