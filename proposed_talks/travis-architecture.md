# 10k Projects, One CI

Imagine a single CI setup running tests for more than 10.000 projects. What would such a setup look like? How would you deal with all the load?

Those are exactly the issues the Travis CI team had to face when building a Distributed Continous Integrations System for the Open Source community.

Travis CI started as a single GitHub project, containing a Ruby on Rails application and a Resque background task. Compare that to 12 months later, where Travis is now four separate deployable apps, uses two different Rubies (1.9.2 and jruby), and comprises a total of 10 GitHub projects.
