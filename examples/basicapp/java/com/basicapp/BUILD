load("@rules_android//android:rules.bzl", "android_binary", "android_library")

android_binary(
    name = "basic_app",
    manifest = "AndroidManifest.xml",
    deps = [":basic_lib"],
)

android_library(
    name = "basic_lib",
    srcs = ["BasicActivity.java"],
    manifest = "AndroidManifest.xml",
    resource_files = glob(["res/**"]),
    deps = [
        "@example_deps//:androidx_lifecycle_lifecycle_viewmodel",
        "@example_deps//:androidx_lifecycle_lifecycle_viewmodel_ktx",
        "@example_deps//:androidx_lifecycle_lifecycle_viewmodel_savedstate",
        "@example_deps//:com_squareup_leakcanary_leakcanary_android",
        "@example_deps//:com_squareup_leakcanary_leakcanary_android_core",
        "@example_deps//:com_squareup_leakcanary_leakcanary_android_instrumentation",
        "@example_deps//:com_squareup_leakcanary_leakcanary_android_utils",
        "@example_deps//:com_squareup_leakcanary_leakcanary_object_watcher",
        "@example_deps//:com_squareup_leakcanary_leakcanary_object_watcher_android",
        "@example_deps//:com_squareup_leakcanary_leakcanary_object_watcher_android_androidx",
        "@example_deps//:com_squareup_leakcanary_leakcanary_object_watcher_android_core",
        "@example_deps//:com_squareup_leakcanary_leakcanary_object_watcher_android_support_fragments",
        "@example_deps//:com_squareup_leakcanary_plumber_android",
        "@example_deps//:com_squareup_leakcanary_plumber_android_core",
        "@example_deps//:com_squareup_leakcanary_shark",
        "@example_deps//:com_squareup_leakcanary_shark_android",
        "@example_deps//:com_squareup_leakcanary_shark_graph",
        "@example_deps//:com_squareup_leakcanary_shark_hprof",
        "@example_deps//:com_squareup_leakcanary_shark_log",
    ],
)
