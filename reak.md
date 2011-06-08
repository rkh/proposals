# Smalltalk On Rubinius - or How To Implement Your Own Programming Language

Programming languages must be implemented in Java or C, everybody knows this.
Sure, a prototype in Ruby, but that would be unusable. After all, Ruby is made
for web development, right? Hard tasks, like implementing a compiler, have to
happen in far more manly languages. But wait, the Rubinius compiler is written
completely in Ruby, and it seems to get pretty decent performance, maybe we
can use that.

In this talk, we will explore the possibilities of using the Rubinius compiler
tool chain to implement our own programming language targeting the Rubinius
VM. We get all the hard work that went into Rubinius for free and above all,
can do the heavy lifting in Ruby, everyone's favorite programming language.

As an example we'll use Reak, a Smalltalk implementation running on Rubinius.
