# Nice Registry

This is an open-source GitHub organization consisting of packages for consuming
npm registry metadata.

## Why?

These modules mostly exist because npm, Inc. does not provide a public API
for collecting registry metadata. Streaming content from the public CouchDB
replication endpoint is about all we (the public) can do for now.

There is a ton of useful package metadata in the npm registry, but if
you're not an expert with CouchDB it can be pretty difficult to access. Back in
early 2015, npm Inc created a
[private internal registry API](https://github.com/npm/public-api) that is
accessible exclusively to the npm website and npm CLI, and there are
[no signs](https://github.com/npm/public-api/issues) of that API becoming
publicly available any time soon.

## Code of Conduct

This project adheres to the
[Contributor Covenant](http://contributor-covenant.org/), a code of conduct for
open source projects.

> be overt in our openness, welcoming all people to contribute, and pledging in return to value them as human beings and to foster an atmosphere of kindness, cooperation, and understanding.

## Contributing

Projects in this organization follow the [open open source](http://openopensource.org/)
contribution model:

> Individuals making significant and valuable contributions are given commit-access to the project to contribute as they see fit. This project is more like an open wiki than a standard guarded open source project.

## Automation

Many of the modules in this org are self-updating. They have [release scripts](https://github.com/nice-registry/owners/blob/8a7002c4cf85b2834266cbcdd816523e02e5ffbe/script/release.sh)
that run hourly or daily using
[Heroku Scheduler](https://devcenter.heroku.com/articles/scheduler), on dynos
that have npm and GitHub authentication credentials baked in.

For more details on this automation technique, see the
[Sweet Sensation of Automation](http://zeke.sikelianos.com/npm-and-github-automation-with-heroku/)
blog post.
