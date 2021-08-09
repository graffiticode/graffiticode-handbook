I've started using [ESLint](https://eslint.org), and I like it. Javascript linters have come a long way in recently years, and I think we should start using one to keep our code legible and help enforce best practices.

Rather than reinvent the proverbial wheel, I suggest we use [AirBnB's Style Guide](https://github.com/airbnb/javascript) as a starting point. Google has a popular one too, but at first blush AirBnB's seems less draconian while being consistent with my preferences. It also calls out the ESLint rules that checks many of its guidelines.

Once we agree on the base style guide, we can call out and possibly modify rules as we see fit. I suggest we start with a minimal set of ESLint enforceable rules and incrementally add to them over time. Eventually, PRs and other commits to master should be lint free.
