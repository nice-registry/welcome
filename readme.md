# Nice Registry

This is an open-source GitHub organization consisting of packages for consuming
npm registry metadata.

## Why?

These modules mostly exist because npm, Inc. does not provide a public API
for collecting registry metadata. Streaming content from the public CouchDB
replication endpoint is about all we (the public) can do for now.

## Open Open Source

This org adheres to the [open open source](http://openopensource.org/)
contribution model:

> Individuals making significant and valuable contributions are given commit-access to the project to contribute as they see fit. This project is more like an open wiki than a standard guarded open source project.

## Automation

Many of the modules in this org are self-updating. They have a release script
that runs periodically on a Heroku instance that has GitHub and npm credentials
baked in.

For more info on this technique, see the [Sweet Sensation of Automation](http://zeke.sikelianos.com/npm-and-github-automation-with-heroku/)
blog post.
