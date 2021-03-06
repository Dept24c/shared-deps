## 0.2.8 - 4 Jan 2017

Dependencies defined inside dependency sets are now automatically non-transitive.
Instead, dependency sets should extend other dependency sets to provide transitive
dependencies.

## 0.2.7 - 1 Apr 2016

Recompute dependencies from the base version of the project (before profiles are applied).
This may cause incompatibilities with other plugins that modify the dependencies, but
does a better job in other cases.

[Closed Issues](https://github.com/walmartlabs/shared-deps/issues?q=milestone%3A0.2.7+is%3Aclosed)

## 0.2.6 - 22 Jan 2016

The list of known dependency ids, output when an unknown dependency id is encountered,
is now output in multiple columns.

The plugin now includes a `viz-deps` task; this will generate a visualization
of the project's dependency graph, as a PDF file.

## 0.2.5 - 16 Dec 2015

Adding caching for speed improvements under very large projects.

## 0.2.4 - 30 Nov 2015

Ensure each profile is processed just once.

Project names are reported fully qualified with namespace, when one is provided.

Fix a number of issues with dependencies vs. pom.xml generation.
There are still outstanding issues with pom.xml generation.

## 0.2.3 - 27 Nov 2015

Properly handle dependencies across profiles so that a correct pom.xml
may be generated. Previously, dependency sets from all modules were merged
into the base profile, which meant that testing dependencies appeared
in the pom.xml (they should be excluded).

## 0.2.2 - 25 Nov 2015

Automatically locate sibling projects and establish them as sharable
dependencies.

Improved reporting of unknown dependency ids.

## 0.2.1 - 20 Nov 2015

First public release.
Improvements to documentation.

## 0.2.0 - 9 Nov 2015

Rename "categories" to "sets".
Fix a bug where a dependencies.edn file more than one directory above
the project root directory caused an exception.

## 0.1.0 - 6 Nov 2015

Initial release.
