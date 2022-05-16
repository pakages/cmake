# CMake

Built with pakages!

![https://raw.githubusercontent.com/syspack/pakages/main/docs/assets/img/paks.png](https://raw.githubusercontent.com/syspack/pakages/main/docs/assets/img/paks.png)

> This is a [pakages](https://github.com/syspack/pakages) repository, meaning the builds are run automatically via the package file here.

This is the first development respository to design the idea around building, testing, and releasing
a package from the same repository. A test will simply not pass if it cannot build.
Our goals for this setup include:

1. Allowing for install from the Gitub URI
2. Adding actions / workflows here to build and deploy
3. Adding consistent ability to test

Given that the install here uses Paks (e.g., the other repos) it should be the case
that when, for example, singularity is updated, the new version is available for use. What we will
need to think about is how to handle cases where a new dependency doesn't allow an old one
to build - we will need some logic wit paks to retry with a previous one. This obviously can
get complicated with many dependencies!
