load("@bazel_sonatype//:defs.bzl", "sonatype_java_export")

sonatype_java_export(
    name = "bsp",
    srcs = glob(["*.java"]),
    maven_coordinates = "org.jetbrains.bsp:bazel-bsp:3.0.0",
    maven_profile = "org.jetbrains",
    pom_template = "//server/src/main/resources:pom.xml",
    resources = ["//log4j_config"],
    visibility = ["//visibility:public"],
    runtime_deps = [
        "//commons",
        "//install:install-lib",
        "//server/src/main/java/org/jetbrains/bsp/bazel/server",
    ],
)
