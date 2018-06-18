workspace(name="bazelswiftproto")

git_repository(
    name = "bazel_skylib",
    remote = "https://github.com/bazelbuild/bazel-skylib.git",
    tag = "0.4.0",
)

# git_repository(
#     name = "build_bazel_rules_swift",
#     remote = "https://github.com/bazelbuild/rules_swift.git",
#     # commit = "a02d1b58d1128d8c038cffebfe14dfbf2abd3e77",
#     tag = "0.2.0",
# )

local_repository(
    name = "build_bazel_rules_swift",
    path = "../rules_swift",
)

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()
