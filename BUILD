load("@rules_cc//cc:defs.bzl", "cc_library")
load("@rules_cc//examples:experimental_cc_shared_library.bzl", "cc_shared_library")

cc_library(
    name = "a",
    srcs = ["a.cc"],
    # linked_statically_by = ["//:a_so"],
    linked_statically_by = [":a_so"],
)

cc_shared_library(
    name = "a_so",
    exports = [":a"],
)
