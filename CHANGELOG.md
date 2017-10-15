# Change Logs
All notable changes to the "minecraft-json-schemas" project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html)

## [Unreleased]

## [v0.1.2] - 2017-10-15
 - Important Bugfix update
### Fixed
 - Property not allowed error
    - Due to `"additionalProperties":false` being outside `oneOf`s rather than inside
    - Property tree is not automatically collapsing
    - Had to remove `"additionalProperties":false` for text components, as it is not possible to block additional properties for text components without moving all parts which can apply to all component types 


## [v0.1.1] - 2017-10-11
 - Bugfix update 
### Fixed
 - Incorrect references to json_component in shared definition
 - Only allows functions and conditions with a `minecraft:` namespace in loot tables, as even the vanilla loot tables don't use it
 - Property not defined error

## v0.1.0 - 2017-10-10
- Initial release
### Added
 - advancement support
 - loot table support
 - `pack.mcmeta` support
 - `sounds.json` support
 - other `.mcmeta` file support

 [Unreleased]: https://github.com/Levertion/minecraft-json-schemas/compare/v0.1.2...HEAD
 [v0.1.2]: https://github.com/Levertion/minecraft-json-schemas/compare/v0.1.1...v0.1.2 
 [v0.1.1]: https://github.com/Levertion/minecraft-json-schemas/compare/v0.1.0...v0.1.1