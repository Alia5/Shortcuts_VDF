[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Issues](https://img.shields.io/github/issues/Alia5/Shortcuts_VDF)](https://github.com/Alia5/Shortcuts_VDF/issues)

# Steam shortcuts.vdf parser

A header only c++20 parser/write for Steams binary shortcuts.vdf format.

## Usage

```c++
    auto shortcuts = VDFParser::Parser::parseShortcuts(path_to_shortcuts_vdf);
    shortcuts[0].appname = "MyChangedShortcut";
    auto written = VDFParser::Parser::writeShortcuts(path_to_shortcuts_vdf, shortcuts);
```


## License

```
Copyright 2021-2022 Peter Repukat - FlatspotSoftware

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Deps

https://github.com/nlohmann/fifo_map