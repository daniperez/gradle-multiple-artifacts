gradle-multiple-artifacts
=========================

Example of code using gradle for delivering multiple artifacts. Unfortunately not working at all.

The master branch contains a library publishing the "api" config with a single dependency and the branch
```client``` contains a library that would make use of that config.

Publishing the library works: the scope of the single dependency is set to "api", but then
the ```client``` is not able to find it. I tried setting the scope and classifier element in the POM without
success.

You can generated the POM file with ```./gradlew uploadArchives```. The pom file can be found in ```build/poms```.
