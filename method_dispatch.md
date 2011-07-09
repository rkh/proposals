# Message in a bottle

What does really happen when we call a method? How do the different Ruby
implementations actually figure out what code to execute? What plumbing is
going on under the hood to get a speedy dispatch? In this talk we will have a
look at the internals of the four major Ruby implementations - 1.8, 1.9, JRuby
and Rubinius, focusing on their dispatch. From look-up tables and call site
caches, to inlining and what on earth is invokedynamic? Expect C, C++, Java,
and, of course, Ruby code. But fear not, all will be explained!

# Why this topic?

I think most Ruby developers do not take a look under the hood and figure out
what is really going on after the Ruby code got compiled to Byte code. This
talk would lay an foundation for a solid understanding of Ruby and VMs in
general and might help understanding performance issues with common Ruby
patterns, lower the barrier for working on Ruby itself or at least to give an
interesting perspective on what Ruby is actually doing.

RubyConf is the perfect occasion, since this is not a web related talk, nor
does it just present some library, but is a talk for everyone even remotely
interested in Ruby itself.

I have not given this talk before. Brian Ford (Rubinius) and Charles Nutter
(JRuby) will help me prepare the talk.
