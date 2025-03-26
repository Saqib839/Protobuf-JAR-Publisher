This repository stores Protocol Buffer (.proto) schemas and compiles them into Java classes using Maven. The resulting Maven artifact is published via GitHub Packages for easy integration into Java applications.

## Compile and push jar package

``mvn clean install``

Note: Make sure your github username and PAT configured in .github/maven-settings/settings.xml
``mvn clean deploy --settings .github/maven-settings/settings.xml``


## use this to inspect the jar created 

``jar tf target/proto-artifact-1.0.0.jar``