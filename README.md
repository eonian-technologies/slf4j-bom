## SLF4J BOM
Bill of materials for SLF4J.

## Usage
In your parent POM or project POM, add the BOM to the `dependencyManagement` section:
```
<dependencyManagement>
    <dependencies>
        ...
        <dependency>
            <groupId>com.eoniantech.build</groupId>
            <artifactId>slf4j-bom</artifactId>
            <version>1.7.25</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency> 
        ...
    </dependencies> 
<dependencyManagement>
```

Then, in the `dependencies` section of your project POM, depend on specific slf4j components without the version:

```
<dependencies>
    ....
    <dependency>
        <groupId>org.slf4j</groupId>
        <artifactId>slf4j-api</artifactId>
    </dependency>
    <dependency>
        <groupId>org.slf4j</groupId>
        <artifactId>jcl-over-slf4j</artifactId>
    </dependency>
    <dependency>
        <groupId>org.slf4j</groupId>
        <artifactId>jul-to-slf4j</artifactId>
    </dependency>
    ...
</dependencies>   
