load("@io_bazel_rules_docker//cc:image.bzl", "cc_image")
load("@io_bazel_rules_docker//container:container.bzl", "container_image", "container_layer")

cc_image(
    name = "io3ded_image",
    binary = "@ioquake3//:ioq3ded",
)

container_layer(
    name = "baseq3_layer",
    directory = "/app/baseq3",
    files = [
        "@baseq3_pak0pk3//file",
        "@baseq3_pak1pk3//file",
        "@baseq3_pak2pk3//file",
        "@baseq3_pak3pk3//file",
        "@baseq3_pak4pk3//file",
        "@baseq3_pak5pk3//file",
        "@baseq3_pak6pk3//file",
        "@baseq3_pak7pk3//file",
        "@baseq3_pak8pk3//file",
    ],
)

container_image(
    name = "server_image",
    base = "io3ded_image",
    layers = [
        ":baseq3_layer",
    ],
)
