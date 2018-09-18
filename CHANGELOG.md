# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## API
The API consists of all public Kotlin types from `com.atlassian.performance.tools.aws.api` and its subpackages:

  * [source compatibility]
  * [binary compatibility]
  * [behavioral compatibility] with behavioral contracts expressed via Javadoc

[source compatibility]: http://cr.openjdk.java.net/~darcy/OpenJdkDevGuide/OpenJdkDevelopersGuide.v0.777.html#source_compatibility
[binary compatibility]: http://cr.openjdk.java.net/~darcy/OpenJdkDevGuide/OpenJdkDevelopersGuide.v0.777.html#binary_compatibility
[behavioral compatibility]: http://cr.openjdk.java.net/~darcy/OpenJdkDevGuide/OpenJdkDevelopersGuide.v0.777.html#behavioral_compatibility

### POM
Changing the license is breaking a contract.
Adding a requirement of a major version of a dependency is breaking a contract.
Dropping a requirement of a major version of a dependency is a new contract.

## [Unreleased]
[Unreleased]: https://bitbucket.org/atlassian/ssh/branches/compare/master%0Drelease-1.0.0

### Added
- Add `TextCapacityMediator(region: Regions)`.

### Fixed
- Bump AMI image version and improve error message. Fix [JPERF-103].

[JPERF-103]: https://ecosystem.atlassian.net/browse/JPERF-103

### Deprecated
- Deprecate `TextCapacityMediator()`.

## [1.0.0]
[1.0.0]: https://bitbucket.org/atlassian/ssh/branches/compare/master%0Drelease-0.0.3

### Changed
- Define public API for the module.
- Use stable APT APIs.
- Opt in for the Nanny.

### Fixed
- Add this changelog.

## [0.0.3] - 2018-08-29
[0.0.3]: https://bitbucket.org/atlassian/ssh/branches/compare/release-0.0.3%0Drelease-0.0.2

### Fixed
- Remove only stacks which "lifespan" tag.
- Don't send requests to AWS while creating Aws object.

## [0.0.2] - 2018-08-29
[0.0.2]: https://bitbucket.org/atlassian/ssh/branches/compare/release-0.0.2%0Drelease-0.0.1

### Added
- License.

## [0.0.1] - 2018-08-22
[0.0.1]: https://bitbucket.org/atlassian/ssh/branches/compare/release-0.0.1%0Dinitial-commit

### Added
- Migrate aws-resources from [JPT submodule].
- Add [README.md](README.md).
- Configure Bitbucket Pipelines.

[JPT submodule]: https://stash.atlassian.com/projects/JIRASERVER/repos/jira-performance-tests/browse/aws-resources?at=cb909508d9c504d7126d68af9c72087f5822ff2b