[Yelp Playground](https://github.com/Yelp/pgctl) ``pgctl``
-----

``pgctl`` is an MIT Licensed tool to manage developer “playgrounds”.

Often projects have various processes that should run in the backround (services) during development. These services amount to a miniature staging environment that we term playground. Each service must have a well-defined state at all times (it should be starting, up, stopping, or down), and should be independantly restartable and debuggable.

``pgctl`` aims to solve this problem in a unified, language-agnostic framework (although the tool happens to be written in Python).

As a simple example, let’s say that we want a date service in our playground, that ensures our now.date file always has the current date.