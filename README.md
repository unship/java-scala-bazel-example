# scala java cooperation

## scala call java lib
```
# java BUILD
java_library(
    name = "me",
    srcs = ["Mine.java"],
    deps = [],
)

# scala BUILD

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_binary", "scala_test")

scala_binary(
    name = "ScalaMain",
    srcs = glob(["*.scala"]),
    main_class = "com.example.ScalaMain.Main",
    deps = [
        "//src/main/java/com/example/me:me",
    ],
)

```

## java call scala lib

```
# scala BUILD
scala_library(
    name = "scala_me",
    srcs = ["DoubleMe.scala"],
    deps = [
        "//src/main/java/com/example/me:me",
    ]
)

java_import(
    name = "java_me",
    deps = [],
    jars = [":scala_me"],
)

# java BUILD, deps the java_import versin lib

java_binary(
    name = "JavaMain",
    srcs = ["Main.java"],
    main_class = "com.example.JavaMain.Main",
    deps = [
        "//src/main/scala/com/example/me:java_me",
    ]
)

```

# import project to intellij

```
# .bazelproject

directories:
  .
targets:
  //...:all
workspace_type: java
java_language_level: 8

```

# bazel manven deps

```bash
git clone https://github.com/pgr0ss/bazel-deps.git
cd bazel-deps
bazel build //src/main/java/braintree:bazeldeps_deploy.jar
java -jar bazel-bin/src/main/java/braintree/bazeldeps_deploy.jar

bazeldeps junit:junit:4.12


--------- Add these lines to your WORKSPACE file ---------

maven_jar(name = "org_hamcrest_hamcrest_core_1_3", artifact = "org.hamcrest:hamcrest-core:jar:1.3")
maven_jar(name = "junit_junit_4_12", artifact = "junit:junit:jar:4.12")


--------- Add these lines to your BUILD file ---------

java_library(
  name="junit",
  visibility = ["//visibility:public"],
  exports = [
    "@junit_junit_4_12//jar",
    "@org_hamcrest_hamcrest_core_1_3//jar",
  ],
)
```

