package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_binary", "scala_test")

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