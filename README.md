This repository stores Protocol Buffer (.proto) schemas and compiles them into Java classes using Maven. The resulting Maven artifact is published via GitHub Packages for easy integration into Java applications.

## Compile

``mvn clean install``

## Push JAR as github packages
Set user specific maven settings in ~/.m2/settings.xml
``nano ~/.m2/settings.xml``

paste 
    ```<settings>
        <servers>
            <server>
            <id>github</id>
            <username>your-github-username</username>
            <password>YOUR_PERSONAL_ACCESS_TOKEN</password>
            </server>
        </servers>
        </settings>```

setup github username that has read/write access to repositary and Personal Access Token (PAT).

run ``mvn clean deploy``

## use this to inspect the jar created 

``jar tf target/proto-artifact-1.0.0.jar``