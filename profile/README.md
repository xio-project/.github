# xio-project

xio-project is a vertically-integrated storage IO stack designed to support multiple vendor targets. The scope is indicated in the name: the "x" denotes vendor-specific prefixes, while IO spans data access protocols, including file-based interfaces.

This stack addresses the problem of ecosystem fragmentation in the face of developers' desire to innovate in creating features and supporting new platforms.

There are two initiatives in this project: cuFile for files and cuObject for objects.
## Repositories

The github organization has been started with repositories for several projects:

For cuFile:
- **cuFileAPI:** Defines the cuFile API as a unifying interface, extensible to new features and multiple platforms
- **cuFileConformance:** Provides a conformance test suite to ensure interoperability and prevent ecosystem fragmentation.
- **libxFile:** Implements one of potentially multiple user-level libraries that implement cuFile APIs for multiple platforms
- **xFileLinux:** A downstream forked full kernel contains enhancements required to support cuFile and libxFile

For cuObject:
- **cuObjectClientAPI:** Defines the cuObjectClient API as a unifying client-side interface, extensible to new features and multiple platforms
- **cuObjectWireProtocol:** Defines the wire protocol(s) used for accelerated client-server communication
- **cuObjectConformance:** Provides a conformance test suite to ensure interoperability and prevent ecosystem fragmentation.

## Integration Model

All layers are validated together to ensure consistent behavior across supported platforms. 
CI/CD support is delegated to individual platform vendors.

## Usage

The code licenses of each repo cover code contributions and redistribution.

## Status

Founders are currently reviewing governance docs.

Once founders have integrated and validated the layers together and are passing conformance tests, and have set up arrangements for making commits, code will appear in the respective repos. Watch this space!

