# What is sbt-rpm ?

SBT is scala build tool. 
RPM is package manager for Redhat, Centos, Scientific Linux.
sbt-rpm can create rpm package. Using sbt-native-packager's rpm plugin.

# Usage

You can use ordinary sbt command

```bash
docker run -ti --rm wshino/sbt-rpm sbt sbt-version
```

This image is configured with a workdir /app

```bash
docker run -it --rm -v "$PWD:/app" -v "$HOME/.ivy2":/root/.ivy2 -v "$HOME/.sbt":/root/.sbt wshino/sbt-rpm sbt rpm:publish
```

