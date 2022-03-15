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

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_file")

[
    http_file(
        name = name,
        downloaded_file_path = file,
        sha256 = sha256,
        urls = [x.format(file) for x in [
            "https://github.com/nrempel/q3-server/raw/master/baseq3/{}",
            "http://game.pioneernet.ru/dl/q3/files/pk3/{}",
        ]],
    )
    for (name, file, sha256) in [
        ("baseq3_pak0pk3", "pak0.pk3", "7ce8b3910620cd50a09e4f1100f426e8c6180f68895d589f80e6bd95af54bcae"),
        ("baseq3_pak1pk3", "pak1.pk3", "d4ffd60b4b414c3419499e321b6f5c2e933cf082df85823ad2d6ae2f803e1682"),
        ("baseq3_pak2pk3", "pak2.pk3", "ccae938a2f13a03b24902d675181d516a431699701ed88023a307f34b5bcd58c"),
        ("baseq3_pak3pk3", "pak3.pk3", "d03c0a0e06b99f9ecca2be7389f57faed406e85f7c09b9c56afdfa53ba25e312"),
        ("baseq3_pak4pk3", "pak4.pk3", "af5f6d5c82fe4440ae0bb660f0648d1fa1731a9e8305a9eb652aa243428697f1"),
        ("baseq3_pak5pk3", "pak5.pk3", "69f87070ca7719e252a3ba97e6483f6663939c987ede550d1268d4d9a07b45bc"),
        ("baseq3_pak6pk3", "pak6.pk3", "bb4f0ae2bf603b050fb665436d3178ce7c1c20360e67bacf7c14d93daff38daf"),
        ("baseq3_pak7pk3", "pak7.pk3", "de6283ce23e3486a2622c5dbf73d3721a59f24debd380e90f43a97d952fea283"),
        ("baseq3_pak8pk3", "pak8.pk3", "812c9e97f231e89cefede3848c6110b7bd34245093af6f22c2cacde3e6b15663"),
    ]
]
