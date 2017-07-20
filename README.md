MemSQL Progress DataDirect MySQL JDBC Driver Example
====================================================

This example assumes the following things:
1. MemSQL is running on `localhost` and listening on port `3306`.
2. The database `test` has already been created, but is otherwise empty.
3. The Progress DataDirect MySQL driver has been installed and the location of
   the `mysql.jar` file contained in its distribution has been added to the Java
   classpath.
4. There is a user named `root` with an empty password within MemSQL

This example was created using Java 8.

Things that have been tested to work:
* Select statements
* Insert statements
* Parameterized queries (query variable injection)
* Switching databases
* Creating/dropping tables
* Standard MySQL datatype conversions
* MemSQL system variables

This driver does not seem to support the registration of custom type converters
(JSON data, for example), but it is possible to read data out as raw strings and
convert them after extraction.