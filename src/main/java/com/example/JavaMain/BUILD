package(default_visibility = ["//visibility:public"])

java_binary(
    name = "JavaMain",
    srcs = ["Main.java"],
    main_class = "com.example.JavaMain.Main",
    deps = [
        "//src/main/java/com/example/me:me",
        "//src/main/scala/com/example/me:java_me",
    ]
)