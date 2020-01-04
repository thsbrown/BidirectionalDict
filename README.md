# BidirectionalDict

<img alt="GitHub issues" src="https://img.shields.io/github/issues-raw/TwentyFourMinutes/BidirectionalDict?style=flat-square"> <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/TwentyFourMinutes/BidirectionalDict?include_prereleases&style=flat-square"> ![GitHub](https://img.shields.io/github/license/TwentyFourMinutes/BidirectionalDict?style=flat-square)

A simple bidirectional Dictionary for C#. BidirectionalDict targets .Net Standard so it's available to you for .Net Core and .Net Framework.

## About

This package brings a basic implementation of a bidirectional Dictionary with it. A bidirectional Dictionary stores two values which are both unique and can each value can be queried by its related partner. 

## Installation

You can either get this package by downloading it from the NuGet Package Manager built in Visual Studio, in the [releases](https://github.com/TwentyFourMinutes/BidirectionalDict/releases) tab or from the official [nuget.org](https://www.nuget.org) website.

### Basic example

```c#
BiDictionary<int, string> dict = new BiDictionary<int, string>();

dict.TryAdd(0, "Hello World!");

dict.TryGet(0, out string val1);
Console.WriteLine(val1); // HelloWorld!

dict.TryGet("Hello World!", out int val2);
Console.WriteLine(val2); // 0
```


## Features

- C# 8.0 ready
- build upon performance
- compatible with Newtonsoft.JSON

## Planned

- Concurrency support

## Notes

If you feel like something is not working as intended or you are experiencing issues, feel free to create an issue. Also for feature requests just create an issue. For further information feel free to send me a mail to `office@twenty-four.dev` or message me on Discord `24_minutes#7496`.







