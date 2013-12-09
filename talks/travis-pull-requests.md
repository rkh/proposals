# I Hear You Like Pull Requests

If you've ever used it, you've probably fallen in love with Github Pull Requests.

This is the story about adding automatic Pull Request testing to Travis CI. We will explore the depths of Git, GitHub and Travis CI. Expect to learn something about Git internals, undocumented APIs, distributed systems and real world usage of hypermedia. And why it all matters.

When you open or update a Pull Request on GitHub, Travis CI is now able to automatically test the merged version and leave a comment indicating whether all tests still pass or not. This feature allows you to really make use of the GitHub Merge Button without having to fear breaking your master branch. Adding this feature to Travis was not as trivial as it seemed in the beginng. Let me take you on a journey through what actually happens, from opening that Pull Request to [travisbot](https://github.com/travisbot) leaving a comment on your blog.

