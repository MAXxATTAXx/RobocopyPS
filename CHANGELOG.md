# RobocopyPS Release History

## 0.2.6 - 2021-09-02

### Added

* Added new cmdlets Get-RoboItem, Remove-RoboItem,Copy-RoboItem,Move-RoboItem.

### Changed

* Removed all ParameterSetName in Invoke-Robocopy, including IncludeSubDirectories (/s) and IncludeEmptySubDirectories (/e) as they are not mutually exlusive.
* Changed Pester Tests to match Version 5 of Pester.
* Changed help file for Get-Help.
* Changed how we validate source directories.

## 0.2.5 - 2021-08-12

### Added

* Added parameters so the module is in phase with native Robocopy, tested on Windows 10 21H1

### Changed

* Removed some of the forced parameters we use (example /v is not used if -Verbose is not specified)
* Changed some tests to be compatible with Pester version 5
* Changed documentation

### Removed

* Removed some tests


## 0.2.2 - 2019-07-18

### Fixed

* Fixed problem with parameter ExcludeFileName and ExcludeDirectory where you could not specify multiple files/directories.

### Added

* Added functionality to Exclude/IncludeAttribute and Remove/AddAttribute


## 0.2.0 - 2019-07-16

### Changed

* A re-write was done to be able to handle error code better and more precisely. Changes to the function names was also done, Start-Robocopy became Invoke-Robocopy and the internal logic handling output from Robocopy.exe was extracted to Invoke-RobocopyParser.

* All other functions was removed during this release so they can be re-worked to follow the new standard.

## 0.1.0 - 2019-05-30

### Fixed

* No fix as this is the first release

### Added

* Added function Start-Robocopy
* Added function Remove-RoboDirectory

### Changed

* No change as this is first release