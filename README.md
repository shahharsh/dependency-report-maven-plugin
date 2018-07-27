# Dependency Report

## Prerequites

	* Java8 on your path

##Quick start:

	* First build the plugin using follwoing command, this will also run the automated test cases.
		mvnw clean install

	* To run the plugin against a given text file execute
		mvnw  com.netflix.maven.plugins:dependencyreport:1.0.0-1-SNAPSHOT:dependency-report -Dgraphfile="LOCATION OF THE FILE"

### Note:

	* The automation of test runs/executes the whole plugin internally to make sure no runtime errors occur.
	* The test can be added easily by just adding methods to ArtifactList test class.
	* The plugin currently detect a repetative childs but does nothing about it.
	* The case of cyclic dependency is solved using graph traversal technique.
	* Have used takari wrapper to auto install maven for the users.
		https://github.com/takari/maven-wrapper


