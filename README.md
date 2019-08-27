# CodeFormatter

[![Build status](https://ci2.dot.net/job/dotnet_codeformatter/job/master/job/innerloop/badge/icon)](https://ci2.dot.net/job/dotnet_codeformatter/job/master/job/innerloop/)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fjamiecool%2Fcodeformatter.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fjamiecool%2Fcodeformatter?ref=badge_shield)

CodeFormatter is a tool that uses Roslyn to automatically rewrite the source to
follow our coding styles, which are [documented here][corefx-coding-style].

[corefx-coding-style]: https://github.com/dotnet/corefx/blob/master/Documentation/coding-guidelines/coding-style.md

## Prerequisites

In order to build or run this tool you will need to have Microsoft Build Tools
2015 installed.  This comes as a part of [Visual Studio 2015](https://www.visualstudio.com/downloads/download-visual-studio-vs).

## Installation

Download binaries from [GitHub Releases](https://github.com/dotnet/codeformatter/releases)

## Usage

In order get the usage, simply invoke the tool with no arguments:

```
$ .\CodeFormatter.exe
CodeFormatter <project or solution> [<rule types>] [/file:<filename>] [/nocopyright] [/c:<config1,config2> [/copyright:file]
    <rule types> - Rule types to use in addition to the default ones.
                   Use ConvertTests to convert MSTest tests to xUnit.
    <filename>   - Only apply changes to files with specified name.
    <configs>    - Additional preprocessor configurations the formatter
                   should run under.
    <copyright>  - Specifies file containing copyright header.
```

## Contributing

We follow the same contribution process that 
[corefx is using][corefx-contributing].

[corefx-contributing]: https://github.com/dotnet/corefx/wiki/Contributing


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fjamiecool%2Fcodeformatter.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fjamiecool%2Fcodeformatter?ref=badge_large)