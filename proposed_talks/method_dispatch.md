# Message in a bottle (simpler version)

What does really happen when we call a method? How do the different Ruby
implementations actually figure out what code to execute? What plumbing is
going on under the hood to get a speedy dispatch? In this talk we will have a
look at the internals of the the major Ruby implementations, focusing on their
dispatch. From look-up tables and call site caches, to inlining and what on
earth is invokedynamic? Fear not, all will be explained!