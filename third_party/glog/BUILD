licenses(["notice"])

cc_library(
  visibility = ["//visibility:public"],
  name = "glog",
  deps = [
    "//third_party/libunwind:libunwind",
    "//third_party/gflags:gflags",
  ],
  includes = [
    "build/include",
    "glog/src",
  ],
  copts = [
    "-DNO_FRAME_POINTER",
    "-Ithird_party/glog/build/src",
  ],
  srcs = [
    "build/include/glog/logging.h",
    "build/include/glog/raw_logging.h",
    "build/include/glog/vlog_is_on.h",
    "build/src/config.h",
    "glog/src/base/commandlineflags.h",
    "glog/src/base/googleinit.h",
    "glog/src/base/mutex.h",
    "glog/src/glog/log_severity.h",
    "glog/src/stacktrace.h",
    "glog/src/stacktrace_generic-inl.h",
    "glog/src/demangle.cc",
    "glog/src/logging.cc",
    "glog/src/raw_logging.cc",
    "glog/src/signalhandler.cc",
    "glog/src/symbolize.cc",
    "glog/src/utilities.cc",
    "glog/src/vlog_is_on.cc",
  ],
  hdrs = [
    "glog/src/demangle.h",
    "glog/src/mock-log.h",
    "glog/src/symbolize.h",
    "glog/src/utilities.h",
  ],
  linkopts = [
    "-pthread"
  ],
)

cc_test(
  name = "demangle_unittest",
  deps = [
    ":glog",
  ],
  srcs = [
    "glog/src/googletest.h",
    "glog/src/demangle_unittest.cc",
  ],
  copts = [
    "-Ithird_party/glog/build/src"
  ],
)

cc_test(
  name = "logging_unittest",
  deps = [
    ":glog",
  ],
  srcs = [
    "glog/src/config_for_unittests.h",
    "glog/src/googletest.h",
    "glog/src/logging_unittest.cc",
  ],
  copts = [
    "-Ithird_party/glog/build/src"
  ],
)

cc_test(
  name = "symbolize_unittest",
  deps = [
    ":glog",
  ],
  srcs = [
    "glog/src/googletest.h",
    "glog/src/symbolize_unittest.cc",
  ],
  copts = [
    "-Ithird_party/glog/build/src"
  ],
)
