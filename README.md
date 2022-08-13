# setting vscode

add settings to omnisharp vscode settings as modern .net is used

path to dotnet

`/home/ec2-user/.dotnet`

full sdk path

`/home/ec2-user/.dotnet/sdk/6.0.400`

see how to setup here

https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-6/


set PGO and Tiered once

```sh
export DOTNET_TieredPGO=1 
export DOTNET_TieredCompilation=1
```

make change, add benchmark and run 

`dotnet run -c Release -filter "**" --runtimes net6.0`

# install java and maven

`sdk install maven`

```java
mvn archetype:generate \
  -DinteractiveMode=false \
  -DarchetypeGroupId=org.openjdk.jmh \
  -DarchetypeArtifactId=jmh-java-benchmark-archetype \
  -DgroupId=org.benchboy \
  -DartifactId=beatdotnet \
  -Dversion=1.0
```

```
cd test
mvn clean verify

java -jar target/benchmarks.jar
```