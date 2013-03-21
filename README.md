gradle-multiple-artifacts
=========================

Example of code using gradle for delivering multiple artifacts. Unfortunately not working at all.

The master branch contains a library publishing the API config with a single depedency and the branch
```client``` contains a library that would make use of that config.

Publishing the library works: the scope of dependency in the POM file is set to the value of the config, but then
the ```client``` is not able to find it. I tried setting the scope and classifier element in the POM without
success.
