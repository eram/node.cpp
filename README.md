# node.cpp
A NodsJS-like library for C++


# intro
Writing code in C++11 is great - powerful and fast. But looking at projects I've been involved with, some problems I see repeating again and again, making C++11 a pass for most new projects. After programming in TypeScript/NodeJS I think I not better understand what's wring and how to make a C++ base SDK that is kind of much like NodeJS with TypeScript, and would make coding in C++ much more productive and a modern experience. We need to make is easy for newbies to find their head around and get going fast: 80% of developers only ever use 20% of the language features. 
Manifest:
- *Multi-threading be gone*. We need a modern event loop. Writing a multi-threaded application properly, protecting data access and synchronizing operations across threads is hard for devs, resulting with a long stabilization process.
- *Synchronous operations be gone*. Async I/O is easy with lambdas; Thread messages with queueing is so much more efficient. 
- We need *a new STD library*. The existing combination of C-STD, C++STD and C++11-STD, with layers of header files, makes it a cluttered experience and hard to find your head around. It gets even worse with boost library! 
- *OS specifics be gone*. WIN32 and POSIX no more! 
- *Modern:* Strings should be UNICODE/UTF8; JSON-like structures should be built-in; Networking and internet-age encryption should be built-in and easy to use. toString() toHash
- *Generics* (template classes) are hard for a lot of developers. We should keep its usage to a minimum on the STD level.
- *Enforce coding standards*: use camel casing for methods; properties and variables; Pascal casing for types; All-caps for constants; no type referencing in the name (e.g. no “m_pRectXxx”). 
- *Ownership of allocated objects* is norm. Use references not pointers whenever possible >> writing code with std::unique_ptr should be the norm. 
- Being *opinionated* is good. 

