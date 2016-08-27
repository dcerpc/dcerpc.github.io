---
title: Documentation
redirect_from: /documentation.html
---

## Open Group Documentation

[C706](http://www.opengroup.org/onlinepubs/9629399/) is the primary specification for DCE/RPC 1.1. This document describes the concepts, protocol and internal mechanisms of the RPC architecture.

The Open Group also has the [DCE 1.2.2 documentation set](http://www.opengroup.org/bookstore/catalog/t151x.htm)
available for purchase. This contains some useful RPC information,
particularly in the Application Development Guide.

## Microsoft Documentation

Since DCE/RPC is the basis for Windows RPC implementation,
Microsoft provide a lot of useful documentation.

Windows extensions to the DCE/RPC protocols are documented in
[MS-RPCE](http://msdn.microsoft.com/en-us/library/cc243560.aspx).

The [Remote Procedure Call](http://msdn.microsoft.com/en-us/library/aa378651.aspx) section of MSDN provides a wealth
of information about the Windows RPC implementation.

The O'Reilly [Microsoft RPC programming guide](http://openlibrary.org/books/OL555525M/Microsoft_RPC_programming_guide) is a nice
introduction to RPC programming on Windows. Most of it can be
directly applied to DCE/RPC just by changing the function names.

## Other Documentation

The [RPC Internals](rpc-internals.pdf) document is
dated and incomplete, but provides a useful insight into some of
the source code architecture and conventions.

The [porting guide](rpc-porting.pdf) contains some historical information
about porting DCE/RPC to new platforms. It's not particularly
relevant anymore, but it occasionally explains some of the rationale
for the strange things that you find in the source.
