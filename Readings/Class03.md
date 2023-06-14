# File and Stream I/O

File and Stream I/O is an important topic because it relates to the handling of data from external sources and storage. And mastering it will empower us to develop applications that can handle input/output operations efficiently and securely.

It Refers to the transfer of data either to or from a storage medium. The System.IO namespaces contain types that enable reading and writing, on data streams and files

## Files and directories

You can use the types in the System.IO namespace to interact with files and directories.

## Streams

The abstract base class Stream supports reading and writing bytes. 
Streams involve three fundamental operations:

- Reading - transferring data from a stream into a data structure, such as an array of bytes.

- Writing - transferring data to a stream from a data source.

- Seeking - querying and modifying the current position within a stream.

### Readers and writers

The System.IO namespace enables encoding conversion between characters and bytes for reading and writing streams.

### Asynchronous I/O operations

With synchronous I/O operations, the UI thread is blocked until the resource-intensive operation has been completed.

### I/O and security

When using System.IO classes, adhere to OS security requirements and manage access control lists (ACLs) for file security. Avoid using physical file paths in internet-based code. Be cautious when sharing streams with less-trusted code.

## Things I want to know more about

- How to handle exceptions and error handling in File and Stream I/O operations.
- Real-world examples and use cases of File and Stream I/O in different applications and domains.