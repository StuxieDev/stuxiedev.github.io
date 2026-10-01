# Changelog

All notable changes to stuxiedev.github.io are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## v1.1.1

### Changed

- The redirect goes to `https://stuxie.dev/` instead of `https://www.stuxie.dev/`

## v1.1.0

### Added
- StuxieDev icon in the README header, plus a one-line description of what the repo does.
- GitHub Actions CI (`.github/workflows/ci.yml`) checking the key repo files exist, HTML parses with no broken local links, workflow YAML is valid, and `VERSION.md` has a matching `CHANGELOG.md` release heading.
- Release workflow (`.github/workflows/release.yml`) that publishes a GitHub Release when a `vX.Y.Z` tag is pushed, with notes taken from the matching `CHANGELOG.md` section.

## v1.0.1

### Fixed
- GitHub Pages was using the legacy branch-deploy build system, which can silently stop auto-deploying with no error recorded anywhere (discovered on SeasonalOverlaysLibrary — its live site served stale content for over an hour with no visible failure). Switched to GitHub Actions-based Pages deployment (`.github/workflows/pages.yml`), making every deploy an ordinary, observable CI run instead.

## v1.0.0

### Added
- First version-tracked release of this GitHub Pages redirect repo — `VERSION.md`/`CHANGELOG.md`/`CONTRIBUTING.md`/`commit.sh`+`commit.bat` added, following the standard release-flow convention used across other StuxieDev repos
