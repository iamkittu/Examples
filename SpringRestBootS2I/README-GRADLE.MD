### Eclipse
`````
gradle cleanEclipseClasspath eclipse
`````

### Clean Build
`````
gradle clean build
`````


### Clean Build skipTests
`````
gradle clean build -x test --stacktrace --warning-mode all
`````

### boot run
`````
gradle clean bootRun -Dserver.port=8080
`````

### execute via war
`````
java -jar build/libs/springrestboots2i.war --server.port=8080 &
`````

### check process
`````
ps -ef | grep springrestboots2i.war | awk '{print $2}'
netstat -lntp | grep 8080
`````
