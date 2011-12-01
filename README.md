GoNow
=====

**GoNow** allows using Go like if were a script language.

Internally, it compiles and links the Go file; the executable is saved into a
global directory if *GOROOT* or *GOPATH* is set, else it is saved in the local
directory "*.go"; then, it is run. If that executable does not exist or
its modified time is different than script's, then it's compiled again.

It works into a shared filesystem since it's created a directory for each target
environment.

"GoNow" is specially useful for:

+ Learning
+ Testing of code snippets
+ Administration issues
+ Boot init of operating systems
+ Web developing; by example for the routing
+ Interfaces of database models


## Installation

	goinstall github.com/kless/GoNow/gonow


## Operating instructions

	gonow file.go

To run it using its name, insert in the first line of the Go file:

	#!/usr/bin/env gonow

and set its executable bit:

	chmod +x file.go


## Copyright and licensing

***Copyright 2010  The "GoNow" Authors***  
See file AUTHORS and CONTRIBUTORS.

Licensed under **BSD 2-Clause License**.  
See file LICENSE.


* * *
*Generated by [GoWizard](https://github.com/kless/GoWizard)*

