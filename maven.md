## To set permgen space

```sh
set MAVEN_OPTS=-Xmx512m -XX:MaxPermSize=128m - windows
export MAVEN_OPTS="-Xmx512m -XX:MaxPermSize=128m" - unix
```

## To solve issue maven-archetype-plugin fails with 'Cannot run additions goals." 

```sh
cd %MAVEN_HOME%\bin
mklink mvn.bat mvn.cmd
```

