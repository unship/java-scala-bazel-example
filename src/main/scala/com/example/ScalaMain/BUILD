package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_binary", "scala_test")

scala_binary(
    name = "ScalaMain",
    srcs = glob(["*.scala"]),
    main_class = "com.example.ScalaMain.Main",
    deps = [
        "//src/main/java/com/example/me:me",
        "//src/main/scala/com/example/me:scala_me",
    ],
)
