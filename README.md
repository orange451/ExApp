# ExApp
Example Applications for JadeFX with GLFW/MiniJVM

https://github.com/orange451/JadeFX

# Deploy
For ios deployment, see: https://github.com/orange451/jadefx_minijvm_ios

# Sample POM
```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<groupId>org.minijvm</groupId>
	<artifactId>ExApp</artifactId>
	<version>1.0-SNAPSHOT</version>
	<packaging>jar</packaging>
	<properties>
		<project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
		<maven.compiler.source>1.8</maven.compiler.source>
		<maven.compiler.target>1.8</maven.compiler.target>
	</properties>

	<dependencies>
		<!-- MiniJVM Runtime -->
		<dependency>
		    <groupId>com.github.orange451</groupId>
		    <artifactId>minijvm_rt</artifactId>
		    <version>master-SNAPSHOT</version>
		</dependency>
		
		<!-- GLFW library --> <!-- required for MiniJVM deployments -->
		<dependency>
		    <groupId>com.github.orange451</groupId>
		    <artifactId>glfw_gui</artifactId>
		    <version>master-SNAPSHOT</version>
		</dependency>
		
		<!-- JadeFX UI library -->
		<dependency>
			<groupId>com.github.orange451</groupId>
			<artifactId>JadeFX</artifactId>
			<version>master-SNAPSHOT</version>
		    <exclusions>
		        <exclusion>
		            <groupId>*</groupId>
		            <artifactId>*</artifactId>
		        </exclusion>
		    </exclusions>
		</dependency>
        
		<dependency>
			<groupId>org.joml</groupId>
			<artifactId>joml</artifactId>
			<version>1.9.25</version>
		</dependency>	
	</dependencies>
</project>
```
