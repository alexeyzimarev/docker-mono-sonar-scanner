# Docker image for Mono and SonarQube scanner

If you want to use SonarQube to run static analysis on C#, you
need to run Sonar Scanner for MSBuild. However, Mono Docker image 
contains no JVM, so if you download the scanner and try to run it inside
the container, it will fail.

This is a pre-made image, where both Mono and Sonar Scanner for MSBuild
are present, with all required dependencies.

You can use this image to run your builds, instead of the default Mono image.

```
docker pull azimarev/mono-sonarqube-scanner
```
