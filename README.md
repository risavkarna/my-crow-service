# Just jib it

```shell
mvn -Pprod verify com.google.cloud.tools:jib-maven-plugin:dockerBuild
```

This will build your 3 docker images (API Gateway, Store, Blog). Then in the `docker-compose` directory run

```shell
docker-compose up -d
```


**Note:** Install maven if it's not already installed (e.g. using [SDKMAN:](https://sdkman.io/install) `sdk install maven`)
