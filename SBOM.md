# Source SBOM

**Initial source snapshot, not a release report.** Source commit `53782729641ff38ec1c338122b59b537774e82e9` predates the tooling commit. Future release reports use exact published tags.

Source repository inventory only; completeness is UNKNOWN. Syft inventories tracked source/package manifests. Gitlinks and declared vendored/model evidence are inspected at immutable pins. CMake declarations are conditional requirements, not resolved installations. This is NOT proof of operating-system packages, static-link closure, build-time resolution, or the contents of release binaries.

Generation: **success**

## Source identity

wave-owl/aprsc `53782729641ff38ec1c338122b59b537774e82e9`

- sbom:role: source-root
- sbom:git-commit: 53782729641ff38ec1c338122b59b537774e82e9
- sbom:git-tree: 98c72aab5c5b9391f6a263530a054c7e18df1598
- sbom:source-repository: https://github.com/wave-owl/aprsc
- sbom:release-tags: []

## Generation errors

None.

## Components and unresolved licenses

| Component | Version | Role | License |
| --- | --- | --- | --- |
| wave-owl/aprsc | 53782729641ff38ec1c338122b59b537774e82e9 | source-root | unresolved |
| Conditional source requirements declared by src/configure.ac | unresolved | conditional-build-runtime-requirement | unresolved |
| Conditional source requirements declared by tests/Makefile | unresolved | conditional-build-runtime-requirement | unresolved |
| Conditional source requirements declared by build/go.mod | unresolved | conditional-build-runtime-requirement | unresolved |
| src/configure.ac and src/Makefile.in: native APRS server, libevent/pthreads/TLS feature checks | unresolved | conditional-build-runtime-requirement | unresolved |
| build/ and tests/ Go modules are tool/test dependencies | unresolved | conditional-build-runtime-requirement | unresolved |
| actions/checkout | v2 | Syft source/package discovery | unresolved |
| actions/setup-go | v5 | Syft source/package discovery | unresolved |
| github.com/hessu/go-aprs-fap | v0.1.0 | Syft source/package discovery | unresolved |
| google.golang.org/protobuf | v1.36.10 | Syft source/package discovery | unresolved |
| .github/workflows/tests.yml | unresolved | Syft source/package discovery | unresolved |
| tests/go/go.mod | unresolved | Syft source/package discovery | unresolved |

License evidence paths/hashes, source manifests, model hashes and conditional
CMake declarations are recorded in SBOM.cdx.json. Declared upstream pins do not
prove vendored equivalence. No dependency installation or build was performed.
