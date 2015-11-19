licenses(["notice"])

cc_library(
  visibility = ["//visibility:public"],
  name = "gflags",
  includes = [
    "build/include",
  ],
  srcs = [
    "build/include/gflags/config.h",
    "gflags/src/mutex.h",
    "gflags/src/util.h",
    "gflags/src/gflags.cc",
    "gflags/src/gflags_completions.cc",
    "gflags/src/gflags_reporting.cc",
  ],
  hdrs = [
    "build/include/gflags/gflags.h",
    "build/include/gflags/gflags_completions.h",
    "build/include/gflags/gflags_declare.h",
    "build/include/gflags/gflags_gflags.h",
  ],
  copts = [
    "-Ithird_party/gflags/build/include/gflags",
  ],
  linkopts = [
    "-pthread",
  ],
)

cc_test(
  name = "gflags_unittest",
  srcs = [
    "gflags/test/config_for_unittests.h",
    "gflags/test/gflags_unittest.cc",
  ],
  copts = [
    "-Ithird_party/gflags/build/include/gflags",  # We need "config.h"
    "-Ithird_party/gflags/gflags/src",
  ],
  deps = [
    ":gflags"
  ],
  size = "small",
)

cc_test(
  name = "gflags_declare_test",
  srcs = [
    "gflags/test/gflags_declare_flags.cc",
    "gflags/test/gflags_declare_test.cc",
  ],
  copts = [
    "-Ithird_party/gflags/build/include/gflags",  # We need "config.h"
    "-Ithird_party/gflags/gflags/src",
  ],
  deps = [
    ":gflags"
  ],
  size = "small",
)

cc_test(
  name = "gflags_strip_flags_test",
  srcs = [
    "gflags/test/config_for_unittests.h",
    "gflags/test/gflags_strip_flags_test.cc",
  ],
  copts = [
    "-Ithird_party/gflags/build/include/gflags",  # We need "config.h"
    "-Ithird_party/gflags/gflags/src",
  ],
  deps = [
    ":gflags"
  ],
  size = "small",
)

