load("@rules_foreign_cc//foreign_cc:defs.bzl", "configure_make")


filegroup(
    name = "all",
    srcs = glob(["**"])
)
configure_make(
    name = "liquid",
    lib_source = ":all",
    configure_in_place = True, 
    autogen = True, 
    autogen_command	= "bootstrap.sh",
    out_shared_libs = [
        "libliquid.so.1",
    ],
    visibility = [
        "//visibility:public"
    ],
)