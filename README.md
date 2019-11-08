# Maven Multi-Module 

Create the parent project:

```
./mvnw archetype:generate \
-DgroupId=br.example \
-DartifactId=maven-multi-module \
-DarchetypeArtifactId=maven-archetype-quickstart \
-DinteractiveMode=false
```
Change the packing to **pom**

```
<packaging>pom</packaging>
```

Create the **jar** module
```
./mvnw archetype:generate \
-DgroupId=br.example \
-DartifactId=module-jar \
-DarchetypeArtifactId=maven-archetype-quickstart \
-DinteractiveMode=false
```

Create the **ear** module
```
./mvnw archetype:generate \
-DgroupId=br.example \
-DartifactId=module-ear \
-DarchetypeArtifactId=maven-archetype-quickstart \
-DinteractiveMode=false
```

Create the **web** module
```
./mvnw archetype:generate \
-DgroupId=br.example \
-DartifactId=module-war \
-DarchetypeArtifactId=maven-archetype-webapp \
-DinteractiveMode=false
```