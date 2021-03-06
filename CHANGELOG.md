# Changelog
All notable changes to the "swarmlib" pypi package will be documented in this file.  
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.14.1...master)

## 2020-12-16 - [v0.14.1](https://github.com/HaaLeo/swarmlib/tree/v0.14.1)

### Fixed

* a bug that caused swarmlib to show an error message instead of the help message when it was invoked without any args ([#36](https://github.com/HaaLeo/swarmlib/issues/36))

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.14.0...v0.14.1)

## 2020-12-04 - [v0.14.0](https://github.com/HaaLeo/swarmlib/tree/v0.14.0)

### Added
* new functions by upgrading [landscapes](https://github.com/nathanrooy/landscapes#readme) to _v0.0.11_

### Fixed
* a bug that caused levy flights to be performed randomly despite `--seed` was enabled.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.13.0...v0.14.0)

## 2020-11-25 - [v0.13.0](https://github.com/HaaLeo/swarmlib/tree/v0.13.0)

### Added
* the _whale optimization algorithm_. After each step the solutions are plotted.

### Fixed
* the upload of release artifacts. Now the bundled pypi packages are added as release artifacts again.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.12.1...v0.13.0)

## 2020-11-17 - [v0.12.1](https://github.com/HaaLeo/swarmlib/tree/v0.12.1)

### Fixed
* swarmlib's appearance on [pypi](https://pypi.org/project/swarmlib). Now the gif renders correctly.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.12.0...v0.12.1)

## 2020-11-16 - [v0.12.0](https://github.com/HaaLeo/swarmlib/tree/v0.12.0)

### Added
* top level flag `--log-level` to set swarmlib's verbosity ([#29](https://github.com/HaaLeo/swarmlib/issues/29)). It can be one of `debug`, `info`, `warning`, `error`, `critical`. Contributed by Nikos Koutsovasilis ([@nkoutsov](https://github.com/nkoutsov)) and happily accepted ????.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.11.0...v0.12.0)

## 2020-11-10 - [v0.11.0](https://github.com/HaaLeo/swarmlib/tree/v0.11.0)

### Added
* visualization of the _alpha_, _beta_ and _delta_ wolves for the grey wolf optimizer ([#14](https://github.com/HaaLeo/swarmlib/issues/14)).
* top level `--seed` flag which allows to set the random bit generator's initial state for reproducible results.

### Changed
* the visualization. Now the initial as well as the end-position are shown unanimated as well.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.10.0...v0.11.0)

## 2020-11-07 - [v0.10.0](https://github.com/HaaLeo/swarmlib/tree/v0.10.0)

### Added
* [landscapes](https://github.com/nathanrooy/landscapes#readme) as a dependency to enable more benchmark functions ([#15](https://github.com/HaaLeo/swarmlib/issues/15)). Contributed by Alex F ([@alxfmpl](https://github.com/alxfmpl)). Thanks a lot ????.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.9.0...v0.10.0)

## 2020-07-21 - [v0.9.0](https://github.com/HaaLeo/swarmlib/tree/v0.9.0)

### Added
* _grey wolf optimizer_ ([#12](https://github.com/HaaLeo/swarmlib/issues/12)). Perform the grey wolf optimization algorithm on one of the selected 2D-functions. Contributed by Nimish Verma ([@NimishVerma](https://github.com/NimishVerma)) and greatly appreciated ????.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.8.1...v0.9.0)

## 2020-04-13 - [v0.8.1](https://github.com/HaaLeo/swarmlib/tree/v0.8.1)

### Fixed
* a bug that caused the ACO algorithm to fail. Due to other third party packages swarmlib now requires `matplotlib<3.2.0`.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.8.0...v0.8.1)

## 2020-04-07 - [v0.8.0](https://github.com/HaaLeo/swarmlib/tree/v0.8.0)

### Added
* the _artificial bee colony_ algorithm. After each step the intermediate solution is plotted.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.7.0...v0.8.0)

## 2020-02-17 - [v0.7.0](https://github.com/HaaLeo/swarmlib/tree/v0.7.0)

### Added
* dark mode. It is enabled via the `--dark` flag.

### Changed
* `--continuous` and `--interval` flags. Both are now top level flags.
* the API of the ant colony optimization.
* the `tsp_file` argument to an option. Now `--tsp-file` is optional. By default the built-in burma14 problem is used.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.6.2...v0.7.0)

## 2020-01-25 - [v0.6.2](https://github.com/HaaLeo/swarmlib/tree/v0.6.2)

### Changed
* cuckoo search visualization: when a nest is abandoned / newly generated color its transition differently.

### Fixed
* cuckoo search visualization: now the abandon transition is mapped to the correct nest.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.6.1...v0.6.2)

## 2020-01-24 - [v0.6.1](https://github.com/HaaLeo/swarmlib/tree/v0.6.1)

### Changed
* cuckoo search: Ensure each nest is assigned a cuckoo position in the update step

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.6.0...v0.6.1)

## 2020-01-24 - [v0.6.0](https://github.com/HaaLeo/swarmlib/tree/v0.6.0)

### Changed
* the visualization of the _firefly algorithm_ and the _cuckoo search_. Now they both include velocities.
* the firefly algorithm including its API. Now it replays the same problem if `--continuous` is set.
* the `--continuous` flag. It requires no parameter anymore.
* the `--two-opt` flag. It requires no parameter anymore.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.5.0...v0.6.0)

## 2020-01-22 - [v0.5.0](https://github.com/HaaLeo/swarmlib/tree/v0.5.0)

### Added
* a feature that performs _particle swarm optimization_ for one of the provided 2D functions. After each step the intermediate solution is plotted.

### Changed
* the API. Now the classes `*Problem` can be directly imported from the `swarmlib` module.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.4.1...v0.5.0)

## 2020-01-19 - [v0.4.1](https://github.com/HaaLeo/swarmlib/tree/v0.4.1)

### Changed
* pypi tags to enhance the package's discoverability.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.4.0...v0.4.1)
## 2020-01-19 - [v0.4.0](https://github.com/HaaLeo/swarmlib/tree/v0.4.0)

### Added
* a feature that enables the _cuckoo search_ for one of the provided 2D functions. After each step the intermediate solution is plotted.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.3.2...v0.4.0)

## 2020-01-09 - [v0.3.2](https://github.com/HaaLeo/swarmlib/tree/v0.3.2)

### Fixed
* a bug in the firefly algorithm that caused the application to crash when the ackley function was selected.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.3.1...v0.3.2)

## 2019-10-30 - [v0.3.1](https://github.com/HaaLeo/swarmlib/tree/v0.3.1)

### Fixed
* a bug in the ACO algorithm that chose the next node by its maximal attractiveness. Now the next node is chosen randomly weighted by its attractiveness

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.3.0...v0.3.1)

## 2018-12-18 - [v0.3.0](https://github.com/HaaLeo/swarmlib/tree/v0.3.0)

### Added
* command line option `--continuous` for the firefly algorithm to indicate, whether the algorithm should run continuously or not
* logging for the current best and overall best intensity found of the firefly algorithm

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.2.0...v0.3.0)

## 2018-12-14 - [v0.2.0](https://github.com/HaaLeo/swarmlib/tree/v0.2.0)

### Added
* a feature that enables the _firefly algorithm_ for one of the provided 2D functions. After each step the intermediate solution is plotted.

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.1.0...v0.2.0)

## 2018-11-29 - [v0.1.0](https://github.com/HaaLeo/swarmlib/tree/v0.1.0)

### Added
* a feature that performs [2-opt](https://en.wikipedia.org/wiki/2-opt) search once on each partial solution after each iteration. It can be disabled via the argument `--two-opt false`.

### Fixed
* an import bug that caused the application to crash instantly

[All Changes](https://github.com/HaaLeo/swarmlib/compare/v0.0.1...v0.1.0)

## 2018-11-23 - [v0.0.1](https://github.com/HaaLeo/swarmlib/tree/v0.0.1)

**Initial Release**

### Added
* a feature that enables solving the Traveling Salesman Problem using the _Ant Colony Optimization_ approach and plots the result afterwards
