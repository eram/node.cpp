# node.cpp
A NodsJS-like library for C++


# intro
Writing code in C++11 is great - powerful and fast. But looking at projects I've been involved with, some problems I see repeating again and again, making C++11 a pass for most new projects. After programming in TypeScript/NodeJS I think I not better understand what's wring and how to make a C++ base SDK that is kind of much like NodeJS with TypeScript, and would make coding in C++ much more productive and a modern experience. 
Wishlist:
- Multi-threading be gone -  we need a modern event loop. Writing a multi-threaded application properly, protecting data access and synchronizing operations across threads is hard for devs, resulting with a long stabilization process.
- Synchronous operations be gone. Thread messages with queueing is so much more efficient. 
- We need a new STD library. The combination of C-STD, C++STD and C++11-STD, with the layer of header files, makes it a cluttered experience and hard to find your head around.
- Strings should be UNICODE from start - UTF8 is the standard these days.
- Generics (template classes) are hard for a lot of developers.
-
