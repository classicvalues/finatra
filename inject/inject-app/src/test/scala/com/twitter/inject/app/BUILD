scala_library(
    sources = ["*.scala"],
    compiler_option_sets = ["fatal_warnings"],
    provides = scala_artifact(
        org = "com.twitter",
        name = "inject-app-tests",
        repo = artifactory,
    ),
    strict_deps = True,
    tags = ["bazel-compatible"],
    dependencies = [
        "//:scala-reflect",
        "3rdparty/jvm/com/google/inject:guice",
        "3rdparty/jvm/com/google/inject/extensions:guice-assistedinject",
        "3rdparty/jvm/net/codingwell:scala-guice",
        "finatra/inject/inject-app/src/main/java/com/twitter/inject/annotations",
        "finatra/inject/inject-app/src/main/scala/com/twitter/inject/app",
        "finatra/inject/inject-app/src/main/scala/com/twitter/inject/app/internal",
        "finatra/inject/inject-core/src/main/scala",
        "util/util-app/src/main/scala",
        "util/util-slf4j-api/src/main/scala/com/twitter/util/logging",
    ],
    exports = [
        "3rdparty/jvm/com/google/inject:guice",
        "finatra/inject/inject-core/src/main/scala",
        "util/util-app/src/main/scala",
        "util/util-slf4j-api/src/main/scala/com/twitter/util/logging",
    ],
)
