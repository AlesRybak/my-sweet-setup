# Some useful Maven commands

## Versions

List project dependencies which could be updated on patch level:

```bash
mvn org.codehaus.mojo:versions-maven-plugin:2.7:display-dependency-updates -DallowMinorUpdates=false -DallowMajorUpdates=false
```


List properties which could be updated on patch level:

```bash
mvn org.codehaus.mojo:versions-maven-plugin:2.7:display-property-updates -DallowMinorUpdates=false -DallowMajorUpdates=false
```


## Security

Check for vulnerable dependencies

```bash
mvn org.owasp:dependency-check-maven:2.1.1:aggregate
```
