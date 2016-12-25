RIO is introduced by Computer Systems: A Programmer's Perspective.

RIO provides two different kinds of functions:

Unbuffered input and output functions. These functions transfer data directly between memory and a file, with no application-level buffering. 
They are especially useful for reading and writing binary data to and from networks.

Buffered input functions. These functions allow you to efficiently read text lines and binary data from a file whose contents are cached in an application-level buffer, 
similar tothe one provided for standard I/O functions such as printf. The buffered RIO input functions are thread-safe and can be interleaved arbitrarily on the same descriptor. 
For example, you can read some text lines from a descriptor, then some binary data, and then some more text lines.
