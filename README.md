# unified-range

Based on the VersionRange [model](https://github.com/apache/maven/tree/master/maven-artifact/src/main/java/org/apache/maven/artifact/versioning) and [spec](https://maven.apache.org/enforcer/enforcer-rules/versionRanges.html) of maven. 

Library to convert semver ranges to unified-range and the over way around.
Currently only supported for comparator semver ranges.

## Install
1. Use pipenv 
`pipenv install unified-range`
or 
2. `pip install unified-range`

## How to use
1. Import the api module:
`from unified_range import api`

2. Convert from semver to the unified range (return VersionRange object):
`ver_rng = api.from_semver(semver_str)`

3. To get the string representation of a VersionRange object:
`version_range_str = str(ver_rng)`

3. Convert from unified spec to semver_str (return str):
`semver = api.to_semver(unified_spec_str)`

4. Convert from spec string to VersionRange objects:
`ver_rng = api.unified_range(unified_spec_str)`
