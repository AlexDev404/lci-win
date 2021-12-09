# LOLCODE for Windows

```python
                    # lci - a LOLCODE interpreter written in C
```
# USAGE

```\
lci.exe [OPTIONS] FILE
Interpret FILE(s) as LOLCODE. Use '-' in place of filename for stdin.
  -h, --help            output this help
  -v, --version         program version


```

# LICENSE

    Copyright (C) 2010-2014 Justin J. Meza

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

# ABOUT

lci is a LOLCODE interpreter written in C and is designed to be correct,
portable, fast, and precisely documented.

    - correct: Every effort has been made to test lci's conformance to the
          LOLCODE language specification. Unit tests come packaged with the lci
          source code.
    - portable: lci follows the widely ported ANSI C specification allowing it
          to compile on a broad range of systems.
    - fast: Much effort has gone into producing simple and efficient code
          whenever possible to the extent that the above points are not
          compromised.
    - precisely documented: lci uses Doxygen to generate literate code
          documentation, browsable here.

This project's homepage is at http://lolcode.org.  For help, visit
http://groups.google.com/group/lci-general.  To report a bug, go to
http://github.com/justinmeza/lci/issues.

Created and maintained by Justin J. Meza <justin.meza@gmail.com>.

# PREREQUISITES

1. You must have CMake installed (www.cmake.org). 

2. Visual Studio 2019 With MSVC Build Tools

# INSTALLATION ON WINDOWS

Go over to releases and download the latest x64 binary.

# BUILD ON WINDOWS

1. Open up [CMake for Windows](https://cmake.org/download/) and locate the directory of the downloaded source code.
  - Configure and set platform to **x64** and generator to **Visual Studio 16 2019**
  - Now Generate the project

2. Once generated, open up the LCI solution file using Visual Studio Code 2019
3. Go to `Project > lci properties > C/C++ > General` and set the Include directory to the base directory of the project
5. Right click on the solution and Build it
6. The compiled LCI Interpretor for Windows should be in either the Debug or Release folder in the project directory (depending on how you built it)
