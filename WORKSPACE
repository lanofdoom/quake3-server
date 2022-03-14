load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_docker",
    sha256 = "59536e6ae64359b716ba9c46c39183403b01eabfbd57578e84398b4829ca499a",
    strip_prefix = "rules_docker-0.22.0",
    urls = ["https://github.com/bazelbuild/rules_docker/releases/download/v0.22.0/rules_docker-v0.22.0.tar.gz"],
)

load(
    "@io_bazel_rules_docker//repositories:repositories.bzl",
    container_repositories = "repositories",
)

container_repositories()

load(
    "@io_bazel_rules_docker//cc:image.bzl",
    _cc_image_repos = "repositories",
)

_cc_image_repos()

http_archive(
    name = "ioquake3",
    build_file = "@//:ioquake3.BUILD",
    sha256 = "05883678af1a496201f99000d7eaa70dfc0eecdb8d268b1fd1b67b6cd10f6621",
    strip_prefix = "ioq3-d77a7d4c90b1df315df6b2a63bb92fd0e8db7e01",
    urls = ["https://github.com/ioquake/ioq3/archive/d77a7d4c90b1df315df6b2a63bb92fd0e8db7e01.zip"],
)
