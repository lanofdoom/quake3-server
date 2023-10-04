load("@rules_pkg//pkg:tar.bzl", "pkg_tar")
load("@rules_oci//oci:defs.bzl", "oci_image", "oci_push")

pkg_tar(
    name = "bin",
    srcs = ["@ioquake3//:ioq3ded"],
    package_dir = "/app",
)

pkg_tar(
    name = "baseq3",
    srcs = ["@baseq3_full//:files"],
    package_dir = "/app/baseq3",
)

oci_image(
    name = "image",
    #architecture = select({
    #    "@platforms//cpu:arm64": "arm64",
    #    "@platforms//cpu:x86_64": "amd64",
    #}),
    base = "@distroless_base",
    entrypoint = ["/app/ioq3ded"],
    #os = "linux",
    tars = [
        ":baseq3",
        ":bin",
    ],
)

oci_push(
    name = "image_push",
    image = ":image",
    remote_tags = ["latest"],
    repository = "ghcr.io/lanofdoom/quake3-server",
)
