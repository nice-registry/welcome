# Nice Registry

The nice registry is a collection of tools that make it easier to work with the npm package registry and learn things from it. 

These projects seek to answer questions like:

- [Who are the most prolific package authors?](https://github.com/nice-registry/owners)
- [What English words are not already taken as package names?](https://github.com/nice-registry/english-words-that-are-not-yet-npm-packages)
- [What are the most popular GitHub API clients?](https://github.com/nice-registry/github-api-modules)
- [How many packages exist?](https://github.com/nice-registry/all-the-package-names/commits/master)
- [How many scoped packages exist?](https://github.com/nice-registry/all-the-package-names/commits/master)
- [What are some popular tools for managing pull requests?](https://github.com/nice-registry/pull-request-modules)
- [Which packages are downloaded the most?](https://github.com/nice-registry/download-counts)
- [What are the GitHub and Twitter handles of a given author?](https://github.com/nice-registry/owner-profiles)
- [What are the most popular CLI tools?](https://github.com/nice-registry/cli-packages)
- [How many packages have a GitHub repo?](https://github.com/nice-registry/all-the-package-repos)
- [What packages are depended on most?](https://github.com/nice-registry/dependent-counts)

## Why?

There is a wealth of useful information in the npm registry, but it's difficult to access.

npm Incorporated **does not have a public API** for collecting or querying registry metadata. 
Back in early 2015, they created a
[private internal registry API](https://github.com/npm/public-api) that is
accessible exclusively to the npm website and npm CLI, and after more than two years there are
[still no signs](https://github.com/npm/public-api/issues) of that API becoming
publicly available.

## Code of Conduct

This project adheres to the
[Contributor Covenant](http://contributor-covenant.org/), a code of conduct for
open source projects.

> be overt in our openness, welcoming all people to contribute, and pledging in return to value them as human beings and to foster an atmosphere of kindness, cooperation, and understanding.

## Contributing

Projects in this organization follow the [open open source](http://openopensource.org/)
contribution model:

> Individuals making significant and valuable contributions are given commit-access to the project to contribute as they see fit. This project is more like an open wiki than a standard guarded open source project.

Many of these repos also adhere to the [Scripts To Rule Them All](https://github.com/github/scripts-to-rule-them-all) pattern popularized by
GitHub:

> If your scripts are normalized by name across all of your projects, your contributors only need to know the pattern, not a deep knowledge of the application. This means they can jump into a project and make contributions without first learning how to bootstrap the project or how to get its tests to run.

> The intricacies of things like test commands and bootstrapping can be managed by maintainers, who have a rich understanding of the project's domain. Individual contributors need only to know the patterns and can simply run the commands and get what they expect.

## Automation

Many of the modules in this org are self-updating. They have [release scripts](https://github.com/nice-registry/owners/blob/8a7002c4cf85b2834266cbcdd816523e02e5ffbe/script/release.sh)
that run hourly or daily using
[Heroku Scheduler](https://devcenter.heroku.com/articles/scheduler), on dynos
that have npm and GitHub authentication credentials baked in.

For more details on this automation technique, see the
[Sweet Sensation of Automation](http://zeke.sikelianos.com/npm-and-github-automation-with-heroku/)
blog post.


## Related Projects

 - https://github.com/johnymontana/npm-graph
