### Welcome to C.ini.
C.ini defines a configuration or ini file format, C structure, and parse code from a single parameter definition file by parsing the definition file multiple times in the C preprocessor with re-defined macros.  Parameters can be added, modified, or deleted editing parameter.def and performing a make.  Backward compatibility to old .ini files is maintained.  Undefined parameters are zero-filled in parsing.  The C 'struct' definition is updated, parse code for reading the parameters in any order is generated, and a input file template is optionally created when the parse code is called.  C.ini makes handling configuration parameters simple and fast in your C/C++ projects.

###Why?
C.ini was developed for scripting ini files for Monte-Carlo simulation tools in C.  C is often the language of choice for MC simulation, but is somewhat tedious with respect to maintaining configuration definition and parsing code.  

### INI file format
The INI file format is reminescent a Fortran namelist file.  Comment lines are officially indicated with a # or % - but in fact any line can be a comment since the parser ignores lines which lack an "=" sign or a recognized parameter to the left of the "=" sign.  Repeated whitespace on the line is ignored, and parameter names must be legal 'C' field names.

### parameter.definition

### Authors and Contributors
Created and contributed by Keith Brodie (@KeithBrodie)

### Support or Contact
Post an issue - I check back when I can.
