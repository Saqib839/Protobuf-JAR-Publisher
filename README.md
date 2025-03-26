## Compile and push jar package

``mvn clean install``

``mvn clean deploy --settings .github/maven-settings/settings.xml``


## use this to inspect the jar created 

``jar tf target/proto-artifacts-1.0.0.jar``