# node.cpp
A NodsJS-like library for C++


# intro
Writing code in C++11/17 is great - powerful and fast. But looking at projects I've been involved with, some problems I see repeating again and again, making C++11/17 a pass for most new projects. After programming in TypeScript/NodeJS I think I've got a better understanding of what is "wrong" and how to make using C++ a modern productive experience - much like NodeJS with TypeScript. We need to make it easy for newbies to find their head around and get going fast: 80% of developers only ever use 20% of the language features. 
Manifest:
- *Multi-threading be gone*. We need a modern event-loop. Writing a multi-threaded application properly, protecting data access and synchronizing operations across threads is hard for devs, resulting with a long stabilization process.
- *Synchronous operations be gone*. Async I/O is easy with lambdas; Thread messages with queueing is so much more efficient. 
- We need *a new STD library*. The existing combination of C-STD, C++STD and C++11-STD, with layers of header files, makes it a cluttered experience and hard to find your head around. It gets even worse with boost library! 
- *OS specifics be gone*. WIN32 and POSIX no more! 
- *Modern:* Strings should be UTF8; JSON-like structures should be built-in; Networking and internet-age encryption should be built-in and easy to use. toString() toHash(); http/s; crypto; websockets etc.
- *Generics* (template classes) are hard for a lot of developers. We should keep its usage to a minimum on the STD level.
- *Package manager:* sharing working code is an excellent way to speed up developement. Solving dependencies and clear versioning is key. No DLL hell!
- *Enforce coding standards*: use camel casing for methods; properties and variables; Pascal casing for types; All-caps for constants; no type referencing in the name (e.g. no “m_pRectXxx”); clear folder sctructure and include hirarchy as part of the standards.
- *Ownership of allocated objects* is norm. Use references not pointers whenever possible >> writing code with std::unique_ptr should be the norm. No need to free(), delete etc.
- Being *opinionated* is good. 


Ref:
https://pagghiu.github.io/dev/A-Node-Like-Api-for-C++-en/
