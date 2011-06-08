# Message in a bottle

What does really happen when we call a method? How do the different Ruby
implementations actually figure out what code to execute? What plumbing is
going on under the hood to get a speedy dispatch? In this talk we will have a
look at the internals of the four major Ruby implementations - 1.8, 1.9, JRuby
and Rubinius, focusing on their dispatch. From look-up tables and call site
caches, to inlining and what on earth is invokedynamic? Expect C, C++, Java,
and, of course, Ruby code. But fear not, all will be explained!
