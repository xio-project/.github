# xio-sig

xio-sig is a vertically-integrated storage IO stack designed to support multiple vendor targets. The scope is indicated in the name: the "x" denotes vendor-specific prefixes, while IO spans data access protocols, including file-based interfaces.

This stack addresses the problem of ecosystem fragmentation in the face of developers' desire to innovate in creating features and supporting new platforms.

## Repositories

The github organization has been started with repositories for four projects:

- **cuFile:** Defines the cuFile API as a unifying interface, extensible to new features and multiple platforms
- **cuFileConformance:** Provides a conformance test suite to ensure interoperability and prevent ecosystem fragmentation.
- **libxPUFile:** Implements one of potentially multiple user-level libraries that implement cuFile APIs for multiple platforms
- **xioLinux:** A downstream forked full kernel contains enhancements required to support cuFile and libxPUFile

## Integration Model

All layers are validated together to ensure consistent behavior across supported platforms. CI/CD support is delegated to individual platform vendors.

## Usage

The code licenses of each repo cover code contributions and redistribution.
