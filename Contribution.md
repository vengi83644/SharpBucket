# How to get started

In order to run the SharpBuckets integration tests you should create OAuth tokens for your Bitbucket account. It is recommended that you create a separate Bitbucket account for developing.

After that create two environment variables for the key and the secret key. They should be named:
- SB_CONSUMER_KEY
- SB_CONSUMER_SECRET_KEY

# Where to get started

The best way to get started is to implement a part of the API that you need but is not covered yet. 

You can check the issues ([here are some](https://github.com/MitjaBezensek/SharpBucket/labels/easy-fix) that should be easy to fix) or look which api calls [are still missing](https://github.com/MitjaBezensek/SharpBucket/blob/master/Coverage.md). A few topics that still need to be covered:
- certain parts of the V2 api
- support for OAuth2 is quite basic
- improve test coverage
- async calls
- logo!

# Guidelines

Just a few guidelines:
- for simple improvements (like adding a missing api call) just submit a PR 
- for architecture and breaking changes please open an issue first and lets discuss what you have planned
- try to stick to the existing formatting as much as possible
- any reformatting should be done in a sepparate PR in order to make it easier to review it

# Continuous integration

The project is using AppVeyor's Continuous Integration Service that is free for open source projects. It is enabled for Pull Requests as well as the main branch. Main branch's current status is:

[![Build status](https://ci.appveyor.com/api/projects/status/jtlni3j2fq3j6pxy/branch/master)](https://ci.appveyor.com/project/MitjaBezenek/sharpbucket/branch/master)

The CI service also runs the Integration tests present in the solution. For now this only covers the public parts of the API. If a build fails you can click on the icon and check what went wrong. You can even see if some test fail.
