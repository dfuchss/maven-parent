# maven-parent
This is a parent pom for my maven projects.

## Usage

Add the following to your pom.xml:
```xml
<parent>
    <groupId>org.fuchss</groupId>
    <artifactId>maven-parent</artifactId>
    <version>X.Y.Z</version>
</parent>
```

For snapshot releases, make sure to add the following repository to your pom.xml:
```xml
<repositories>
	<repository>
		<releases>
			<enabled>false</enabled>
		</releases>
		<snapshots>
			<enabled>true</enabled>
		</snapshots>
		<id>mavenSnapshot</id>
		<url>https://s01.oss.sonatype.org/content/repositories/snapshots</url>
	</repository>
</repositories>
```