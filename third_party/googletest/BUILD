licenses(["notice"])

cc_library(
    name = "gtest",
    srcs = glob(
        ["googletest/googletest/src/*.cc", "googletest/googletest/src/*.h"],
        exclude = ["googletest/googletest/src/gtest-all.cc"]
    ),
    hdrs = glob(["googletest/googletest/include/**/*.h"]),
    includes = [
        "googletest/googletest",
        "googletest/googletest/include",
    ],
    linkopts = ["-pthread"],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "gmock",
    srcs = glob(
        ["googletest/googlemock/src/*.cc", ],
        exclude = ["googletest/googlemock/src/gmock-all.cc",]
    ),
    hdrs = glob(["googletest/googlemock/include/**/*.h", "googletest/googletest/include/**/*.h"]),
    includes = [
        "googletest/googlemock",
        "googletest/googlemock/include",
        "googletest/googletest/include",
    ],
    linkopts = ["-pthread"],
    visibility = ["//visibility:public"],
)
