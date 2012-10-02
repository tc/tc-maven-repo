#tc-maven-repo
http://tommy.chheng.com

## Getting Started
Add to your pom.xml:

```
<repositories>
    <repository>
        <id>tc-maven-repo</id>
        <url>https://github.com/tc/tc-maven-repo/raw/master/releases</url>
    </repository>
</repositories>
```

## Recent artifacts
```
    <dependency>
      <groupId>com.jimplush</groupId>
      <artifactId>goose</artifactId>
      <version>2.1.19</version>
    </dependency>
```

## To deploy a third party jar:
```
mvn deploy:deploy-file
-Durl=file:PATH_TO_LOCAL/src/tc-maven-repo/releases -Dfile=target/lamejb-0.2.0.jar -DgroupId=net.sf -DartifactId=lamejb -Dversion=0.2.0 -Dpackaging=jar
```
