### Welcome to C.ini
C.ini defines a configuration (.cfg,.ini,...) file format, C structure, and parse code from a single parameter definition file.  The parameter definition file is included multiple times in the C preprocessor with re-defined macros performing the work.  Parameters can be added, modified, or deleted editing parameter.def and performing a make.  Backward compatibility to old .ini files is maintained.  Undefined parameters are zero-filled in parsing.  The C 'struct' definition is updated, parse code for reading the parameters in any order is generated, and a input file template is optionally created when the parse code is called.  C.ini makes handling configuration parameters simple and fast in your C/C++ projects.

###Why?
C.ini was developed for defining and maintaining .ini files for Monte-Carlo simulation tools in C.  C is often the language of choice for MC simulation, but is somewhat tedious with respect to maintaining configuration definition and parsing code. Having had to do several times, I wanted a tool to automate the process to the extent I could while remaining usable in any ANSI C environment. With this tool input parameter definitions and parsing can be updated with one file touch.

### INI file format
The INI file format is loosely derived from a Fortran namelist file.  Comment lines are officially indicated with a # or % - but in fact any line without an '=' can be a comment.  The parser ignores any lines which lack a defined field to the left of the '='.  Repeated whitespace on the line is ignored.  Parameter names must be legal 'C' field names.

### parameter.def

### Authors and Contributors
Created and contributed by Keith Brodie (@KeithBrodie)

### Support or Contact
Post an issue - I check back when I can.
