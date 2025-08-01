# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.63] - 2025-07-29
### Fix
Fixes Sarif Markdown value failing to populate the rule provided recommendation value. #697

### Dependencies
Update dependencies 

### Tests
Adds test cases for SarifWriter

## [1.0.62] - 2025-07-23
### Pipelines
Pipeline updates

## [1.0.61] - 2025-07-11
### Pipelines
Pipeline updates

## [1.0.60] - 2025-06-26
### Pipelines
Pipeline updates

## [1.0.59] - 2025-06-10
### Misc (non-code)
Removes old doc publish workflow. 

## [1.0.58] - 2025-06-09
### New Feature
Adds a `vs` output format to leverage the DevSkim CLI as a build task in a csproj.

## [1.0.57] - 2025-05-28
### Fix
Fix an issue handling non-ascii paths when launching LSP in VS Code Extension

### Dependencies
Update Dependencies

## [1.0.56] - 2025-04-14
### Tests
Migrate to MTP

## [1.0.55] - 2025-04-14
### Dependencies
Updates Dependencies

## [1.0.54] - 2025-04-09
### Dependencies
Updates Dependencies

## [1.0.53] - 2025-04-01
### Documentation
Adds a link to the Microsoft Privacy Statement to the Readme.

## [1.0.52] - 2024-12-09
### Dependencies
Updates Dependencies

### .Net Targets
CLI now targets .NET 8.0 and .NET 9.0, .NET 6.0/7.0 targeting removed. DevSkim Library component retains .Net Standard 2.1 support.

## [1.0.51] - 2024-12-09
### Fix
Fix confidence filtering at rule level.

## [1.0.50] - 2024-12-05
### Fix
Fixes #664 handling of options from IgnoreRuleMap when using OptionsJson

### New Functionality
Adds `include-globs` argument to require all scanned files match a specific glob pattern #663.

## [1.0.49] - 2024-12-03
### Rules
Fixed false positives and false negatives in outdated/banned SSL/TLS protocols. #649

## [1.0.48] - 2024-11-20
### Dependencies
Update VS Code Extension Dependencies

## [1.0.47] - 2024-11-12
### Pipeline
Pipeline only changes

## [1.0.46] - 2024-11-05
### Pipeline
Pipeline only changes

## [1.0.45] - 2024-11-01
### Pipeline
Pipeline only changes

## [1.0.44] - 2024-11-01
### Pipeline
Pipeline only changes

## [1.0.43] - 2024-10-29
### Pipeline
Pipeline only changes

## [1.0.42] - 2024-08-26
## Fix
Fixes suppression command to not perturb line breaks, particularly when a file has findings which are not selected for suppression. #631

## [1.0.41] - 2024-08-23
## Rules
Extend the false positive fix for the issue reported in #548 to Sdk-style msbuild projects.

## [1.0.40] - 2024-7-08
## Fix
Fixes extraneous printing of git errors when git ignore checking is enabled during analysis.

## [1.0.39] - 2024-6-26
### Pipelines
Pipeline maintenance.

## [1.0.38] - 2024-6-05
### Incomplete Guidance
Expanded content for rule guidance containing "TO DO"s.

## [1.0.37] - 2024-5-23
### Missing Guidance
Added guidance for several rules such as weak hash algorithm, disabling certificate validation, and TLS client configuration.

## [1.0.36] - 2024-05-21
### Rules
Fix substitution pattern in PHP Request rule.

## [1.0.35] - 2024-5-8
### Pipeline
Pipeline only changes

## [1.0.34] - 2024-3-18
### Pipeline
Pipeline only changes

## [1.0.33] - 2024-3-13
### Fix
Fixes properly setting the default value for the `OutputFileFormat` and `OutputTextFormat` fields when using the `options-json` argument to the analyze command.

## [1.0.32] - 2024-3-04
### Pipeline
Improvement to pipeline to allow rerunning failed deploy jobs.

## [1.0.31] - 2024-2-28
### Sarif Format
Populate additional fields for GitHub Code scanning

### Rules
Populate Confidence values for rules

### Dependencies
Update Dependencies

### Engine
Prioritize confidence value from Pattern level in Issue records but fall back to rule level if not specified.

## [1.0.30] - 2024-1-31
### Pipeline
Additional pipeline fixes

## [1.0.29] - 2024-1-17
### Pipeline
Fix GitHub binary release process

### Dependencies
Update Application Inspector dependency

## [1.0.28] - 2024-1-4
### Fix
Remove trailing period after general guidance URI in output to make it clickable when automatically converted to uri by terminal

### Dependencies
Update dependencies

## [1.0.27] - 2023-12-12
### Pipelines
Move GitHub Release task to last task in publish pipeline.

## [1.0.26] - 2023-12-05
### Dependencies
Update dependencies.

### Framework
Build using .NET 8

## [1.0.25] - 2023-11-10
### Dependencies
Update dependencies. Resolves an issue with some xpath queries via AppInspector Rules engine https://github.com/microsoft/ApplicationInspector/pull/567

## [1.0.24] - 2023-10-10
### Dependencies
Update OmniSharp language server and App Inspector dependencies.

## [1.0.23] - 2023-10-05
### Miscellaneous
Update deployment pipeline version

## [1.0.22] - 2023-09-14
### Dependencies
Update dependencies - incorporate a fix for an issue with JSONPath selection used for matching boolean values. https://github.com/microsoft/ApplicationInspector/pull/561

### Rules
Fix a JSON formatting error in the android debuggable rule

### Miscellaneous
Delete advisory parser script. #586

## [1.0.21] - 2023-09-11
### Dependencies
Update action versions for github workflows.

## [1.0.20] - 2023-08-28
### Fixes
Removes workaround for 404 sarif schema uri

### Dependencies
Updates dependencies to latest.

### VS Extension
Fix ordering of proposed fixes in UX. #582

## [1.0.19] - 2023-08-22
### VS Extension
Fix concurrent access issue with cache storage for fixes. Fix #480

## [1.0.18] - 2023-08-09
### Rules
Fix language filtering on random number generator rules. Fix #468

## [1.0.17] - 2023-08-07
### Rules
Improve HTTP url detection rule to exclude more schema definitions.

## [1.0.16] - 2023-08-04
### Fixes
Fixes an issue with loading settings in the Visual Studio extension.

## [1.0.15] - 2023-07-31
### Rules
Fix false positives reported in #344, #548 and #549.

## [1.0.14] - 2023-07-27
### Fixes
Fixes an issue handling IEnumerable arguments specified with the options-json argument to Analyze.

### Dependencies
Updates RuleEngine dependency to fix an issue with handling matching strings with `//` in languages that use `//` for inline comment format.

## [1.0.13] - 2023-07-24
### Dependencies
Update VS Code Extension Dependencies

## [1.0.12] - 2023-07-24
### Guidance
Updated Guidance for DS126858 

## [1.0.11] - 2023-06-26
### Update Dependency
- Update SemVer dependency in VS Code Extension.

## [1.0.10] - 2023-06-26
### Fixed
- Removed sub scan workspace command in VS Code extension.

## [1.0.9] - 2023-06-26
### Fixed
- Fixed an issue in the VS Code Extension that would try to run the language server with dotnet on the system path instead of the version fetched by the .NET Install Tool extension.

## [1.0.8] - 2023-06-09
### Rules
- Adds new rules and improves precision of some existing rules.

## [1.0.7] - 2023-06-06
### Fixed
- Fixes issue where the CLI global tool package was attempting to run with a mismatched runtime.

## [1.0.6] - 2023-05-25
### Republish
- Republish of 1.0.5 due to a release pipeline error

## [1.0.5] - 2023-05-25
### Added
- Add CHANGELOG.md

### Fixed
- Support ignore-case `i` and multi-line `m` modifiers on the Pattern property of Fixes.

## [1.0.4] - 2023-05-24
### Fixed
- Fixes output sarif returning not applicable fixes

## [1.0.3] - 2023-05-24
### Fixed
- Fixes output sarif for runs with rules with empty string for Recommendation and Description

## [1.0.2] - 2023-05-24
### Fixed
- Fix output sarif for runs with rules with null string for Recommendation and Description

## [1.0.1] - 2023-05-24
This version is a major refactor of DevSkim.

### Added
- Added fix and suppress commands that operate on the output sarif from Analyze and the source code scanned with analyze to apply fixes/suppressions

Usage: 
```bash
devskim analyze -I path/to/source -O myresults.sarif​
devskim fix -I path/to/source -O myresults.sarif --dry-run --all​
devskim suppress -I path/to/source -O myresults.sarif --dry-run --all
```
- Support jsonpath/xpath and ymlpath based rules
- New `--options-json` argument to analyze to specify DevSkim configuration via a JSON file, including ability to Ignore rules only for specific languages
- IDE extensions are now based on a unified C# Language Server, should have better performance and reliability and support new options like user provided Rules/Languages.
- DevSkim Rule format is now an extension of Application Inspector rule format

### Changed
- Input/output files are now named parameters (-I/--source-code and -O/--output-file), not positional parameters

Old: `devskim analyze path/to/src path/to/output.sarif -f sarif`

New: `devskim analyze -I path/to/src -O path/to/out.sarif`
- Sarif is now the default output format for the CLI
- DevSkim targets .NET 6.0 and .NET 7.0
- Rule self tests are now included directly in rule specification (must-match and must-not-match fields) and are checked by the Verify command.
- Visual Studio Extension now targets VS 2022 instead of VS 2019.
- VS Code Extension now requires VSC Engine 1.63 or later

### Removed
- Json is no longer supported as an output format argument to CLI
- Pack, test and catalogue commands removed from CLI

### Fixes
- Rule improvements and DevSkim engine performance and reliablity improvements.
