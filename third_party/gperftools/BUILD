licenses(["notice"])

cc_library(
  name = "profiler",
  visibility = ["//visibility:public"],
  hdrs = [
    "include/gperftools/profiler.h",
    "include/gperftools/heap-profiler.h",
  ],
  srcs = [
    "lib/libprofiler.a",
    "lib/libprofiler.so",
  ],
)

cc_library(
  name = "tcmalloc",
  visibility = ["//visibility:public"],
  hdrs = [
    "include/gperftools/tcmalloc.h",
    "include/gperftools/heap-checker.h",
  ],
  srcs = [
    "lib/libtcmalloc.a",
    "lib/libtcmalloc.so",
  ],
)

cc_library(
  name = "tcmalloc_and_profiler",
  visibility = ["//visibility:public"],
  hdrs = [
    "include/gperftools/heap-checker.h",
    "include/gperftools/heap-profiler.h",
    "include/gperftools/malloc_extension.h",
    "include/gperftools/malloc_extension_c.h",
    "include/gperftools/malloc_hook.h",
    "include/gperftools/malloc_hook_c.h",
    "include/gperftools/profiler.h",
    "include/gperftools/stacktrace.h",
    "include/gperftools/tcmalloc.h",
  ],
  srcs = [
    "lib/libtcmalloc_and_profiler.a",
    "lib/libtcmalloc_and_profiler.so",
  ],
)

cc_library(
  name = "tcmalloc_debug",
  visibility = ["//visibility:public"],
  hdrs = [
    "include/gperftools/heap-checker.h",
    "include/gperftools/tcmalloc.h",
  ],
  srcs = [
    "lib/libtcmalloc_debug.a",
    "lib/libtcmalloc_debug.so",
  ],
)

cc_library(
  name = "tcmalloc_minimal",
  visibility = ["//visibility:public"],
  hdrs = [
    "include/gperftools/heap-checker.h",
    "include/gperftools/tcmalloc.h",
  ],
  srcs = [
    "lib/libtcmalloc_minimal.a",
    "lib/libtcmalloc_minimal.so",
  ],
)

cc_library(
  name = "tcmalloc_minimal_debug",
  visibility = ["//visibility:public"],
  hdrs = [
    "include/gperftools/heap-checker.h",
    "include/gperftools/tcmalloc.h",
  ],
  srcs = [
    "lib/libtcmalloc_minimal_debug.a",
    "lib/libtcmalloc_minimal_debug.so",
  ],
)

#AM_CXXFLAGS = [
#  # Include the generated headers.
#  "-Ithird_party/gperftools/linux-x86_64/src",
#  # Include the source directory
#  "-Ithird_party/gperftools/gperftools/src",
#  "-Wall",
#  "-Wwrite-strings",
#  # "-Woverloaded-virtual",
#  "-Wno-sign-compare",
#  "-fno-builtin-malloc",
#  "-fno-builtin-free",
#  "-fno-builtin-realloc",
#  "-fno-builtin-calloc",
#  "-fno-builtin-cfree",
#  "-fno-builtin-memalign",
#  "-fno-builtin-posix_memalign",
#  "-fno-builtin-valloc",
#  "-fno-builtin-pvalloc",
#  "-Wno-unused-result",
#  "-fno-omit-frame-pointer",
#]
#
#cc_library(
#  name = "logging",
#  copts = AM_CXXFLAGS,
#  hdrs = [
#  ],
#  srcs = [
#    "gperftools/src/base/logging.h",
#    "gperftools/src/base/commandlineflags.h",
#    "gperftools/src/base/basictypes.h",
#    "gperftools/src/base/dynamic_annotations.h",
#    "gperftools/src/third_party/valgrind.h",
#    "gperftools/src/base/logging.cc",
#    "gperftools/src/base/dynamic_annotations.c",
#  ],
#  deps = [
#    ":sysinfo",
#  ]
#)
#
#cc_library(
#  name = "sysinfo",
#  copts = AM_CXXFLAGS,
#  hdrs = [
#    "gperftools/src/base/sysinfo.h",
#    "gperftools/src/getenv_safe.h",
#  ],
#  srcs = [
#    "gperftools/src/base/arm_instruction_set_select.h",
#    "gperftools/src/base/basictypes.h",
#    "gperftools/src/base/commandlineflags.h",
#    "gperftools/src/base/dynamic_annotations.h",
#    "gperftools/src/base/logging.h",
#    "gperftools/src/base/sysinfo.cc",
#    "linux-x86_64/src/config.h",
#  ]
#)
#
#cc_library(
#  name = "spinlock",
#  includes = [
#    "src"
#  ],
#  copts = AM_CXXFLAGS,
#  hdrs = [
#    "gperftools/src/base/spinlock.h",
#    "gperftools/src/base/spinlock_internal.h",
#    "gperftools/src/base/spinlock_win32-inl.h",
#    "gperftools/src/base/spinlock_linux-inl.h",
#    "gperftools/src/base/spinlock_posix-inl.h",
#    "gperftools/src/base/atomicops-internals-macosx.h",
#    "gperftools/src/base/atomicops-internals-linuxppc.h",
#    "gperftools/src/base/atomicops-internals-arm-generic.h",
#    "gperftools/src/base/atomicops-internals-arm-v6plus.h",
#    "gperftools/src/base/atomicops-internals-mips.h",
#    "gperftools/src/base/atomicops-internals-windows.h",
#    "gperftools/src/base/atomicops-internals-gcc.h",
#    "gperftools/src/base/atomicops-internals-x86.h",
#  ],
#  srcs = [
#    "gperftools/src/base/atomicops.h",
#    "gperftools/src/base/googleinit.h",
#    "gperftools/src/base/linux_syscall_support.h",
#    "gperftools/src/base/thread_annotations.h",
#    "gperftools/src/base/spinlock.cc",
#    "gperftools/src/base/spinlock_internal.cc",
#    "gperftools/src/base/atomicops-internals-x86.cc",
#  ],
#  deps = [
#    ":logging",
#    ":sysinfo",
#  ],
#)
#
#cc_library(
#  name = "maybe_threads",
#  copts = AM_CXXFLAGS,
#  srcs = [
#    "linux-x86_64/src/config.h",
#    "gperftools/src/base/basictypes.h",
#    "gperftools/src/base/commandlineflags.h",
#    "gperftools/src/base/logging.h",
#    "gperftools/src/maybe_threads.h",
#    "gperftools/src/maybe_threads.cc",
#  ]
#)
#
#cc_library(
#  name = "raw_printer",
#  copts = AM_CXXFLAGS,
#  hdrs = [
#    "gperftools/src/raw_printer.h"
#  ],
#  srcs = [
#    "linux-x86_64/src/config.h",
#    "gperftools/src/base/basictypes.h",
#    "gperftools/src/base/commandlineflags.h",
#    "gperftools/src/base/logging.h",
#    "gperftools/src/raw_printer.cc"
#  ]
#)
#
#cc_library(
#  name = "stacktrace",
#  copts = AM_CXXFLAGS,
#  hdrs = [
#    "gperftools/src/gperftools/stacktrace.h",
#  ],
#  srcs = [
#    "gperftools/src/stacktrace_impl_setup-inl.h",
#    "gperftools/src/stacktrace_generic-inl.h",
#    "gperftools/src/stacktrace_libunwind-inl.h",
#    "gperftools/src/stacktrace_arm-inl.h",
#    "gperftools/src/stacktrace_powerpc-inl.h",
#    "gperftools/src/stacktrace_powerpc-darwin-inl.h",
#    "gperftools/src/stacktrace_powerpc-linux-inl.h",
#    "gperftools/src/stacktrace_x86-inl.h",
#    "gperftools/src/stacktrace_win32-inl.h",
#    "gperftools/src/stacktrace_instrument-inl.h",
#    "gperftools/src/base/elf_mem_image.h",
#    "gperftools/src/base/vdso_support.h",
#    "gperftools/src/stacktrace.cc",
#    "gperftools/src/base/elf_mem_image.cc",
#    "gperftools/src/base/vdso_support.cc",
#  ],
#  deps = [
#    ":spinlock",
#    "//third_party/libunwind:libunwind",
#  ]
#)
#
#TCMALLOC_CFLAGS = [
#  "-pthread",
#  "-DNDEBUG",
#  # Certain tests require exception, so we didn't disable exception
#  # completely.
#  # "-fno-exceptions",
#] + AM_CXXFLAGS
#
#cc_library(
#  name = "profiler",
#  visibility = ["//visibility:public"],
#  copts = TCMALLOC_CFLAGS,
#  hdrs = [
#    "gperftools/src/profiledata.h",
#    "gperftools/src/profile-handler.h",
#  ],
#  srcs = [
#    "gperftools/src/gperftools/profiler.h",
#    "gperftools/src/gperftools/stacktrace.h",
#    "gperftools/src/getpc.h",
#    "gperftools/src/maybe_threads.h",
#    "gperftools/src/profiler.cc",
#    "gperftools/src/profile-handler.cc",
#    "gperftools/src/profiledata.cc",
#  ],
#  deps = [
#    ":spinlock",
#    ":logging",
#  ]
#)
#
#cc_library(
#  name = "internal",
#  hdrs = [
#  ],
#  srcs = [
#    "gperftools/src/gperftools/malloc_extension.h",
#    "gperftools/src/common.h",
#    "gperftools/src/internal_logging.h",
#    "gperftools/src/system-alloc.h",
#    "gperftools/src/packed-cache-inl.h",
#    "gperftools/src/tcmalloc_guard.h",
#    "gperftools/src/base/commandlineflags.h",
#    "gperftools/src/base/basictypes.h",
#    "gperftools/src/pagemap.h",
#    "gperftools/src/sampler.h",
#    "gperftools/src/central_freelist.h",
#    "gperftools/src/linked_list.h",
#    "gperftools/src/libc_override.h",
#    "gperftools/src/libc_override_gcc_and_weak.h",
#    "gperftools/src/libc_override_glibc.h",
#    "gperftools/src/libc_override_osx.h",
#    "gperftools/src/libc_override_redefine.h",
#    "gperftools/src/page_heap.h",
#    "gperftools/src/page_heap_allocator.h",
#    "gperftools/src/span.h",
#    "gperftools/src/static_vars.h",
#    "gperftools/src/symbolize.h",
#    "gperftools/src/thread_cache.h",
#    "gperftools/src/stack_trace_table.h",
#    "gperftools/src/base/thread_annotations.h",
#    "gperftools/src/common.cc",
#    "gperftools/src/central_freelist.cc",
#    "gperftools/src/page_heap.cc",
#    "gperftools/src/sampler.cc",
#    "gperftools/src/span.cc",
#    "gperftools/src/stack_trace_table.cc",
#    "gperftools/src/static_vars.cc",
#    "gperftools/src/symbolize.cc",
#    "gperftools/src/system-alloc.cc",
#    "gperftools/src/thread_cache.cc",
#    # Others
#  ],
#  copts = TCMALLOC_CFLAGS,
#  deps = [
#    ":spinlock",
#    ":maybe_threads",
#    ":stacktrace",
#  ],
#  linkopts = [
#    "-lm",
#    "-pthread",
#  ],
#  linkstatic = 1,
#)
#
#cc_library(
#  name = "thread_lister",
#  srcs = [
#    "linux-x86_64/src/config.h",
#    "gperftools/src/base/linuxthreads.h",
#    "gperftools/src/base/linux_syscall_support.h",
#    "gperftools/src/base/thread_lister.h",
#    "gperftools/src/base/thread_lister.c",
#    "gperftools/src/base/linuxthreads.cc",
#  ],
#  copts = AM_CXXFLAGS,
#)
#
#HEAP_CHECKER_SRCS = [
#  "gperftools/src/heap-checker.cc",
#  "gperftools/src/heap-checker-bcad.cc"
#]
#
## Malloc_hook contains some hidden symbols that are accessed by some
## other files, as well as tcmalloc.cc and debugallocation.cc, so these
## files need to compiled inside the same cc_library target.
##
## Otherwise we will see the linker would complain: relocation
## R_X86_64_PC32 against undefined hidden symbol
## `_ZN4base8internal10new_hooks_E' can not be used when making a
## shared object
#MALLOC_HOOK_SRCS = [
#  "gperftools/src/base/low_level_alloc.h",
#  "gperftools/src/gperftools/heap-profiler.h",
#  "gperftools/src/addressmap-inl.h",
#  "gperftools/src/malloc_hook-inl.h",
#  "gperftools/src/malloc_hook_mmap_linux.h",
#  "gperftools/src/base/low_level_alloc.cc",
#  "gperftools/src/gperftools/malloc_extension.h",
#  "gperftools/src/gperftools/malloc_extension_c.h",
#  "gperftools/src/gperftools/malloc_hook.h",
#  "gperftools/src/gperftools/malloc_hook_c.h",
#  "gperftools/src/heap-profile-table.cc",
#  "gperftools/src/heap-profiler.cc",
#  "gperftools/src/internal_logging.cc",
#  "gperftools/src/malloc_extension.cc",
#  "gperftools/src/malloc_hook.cc",
#  "gperftools/src/memfs_malloc.cc",
#  "gperftools/src/memory_region_map.cc",
#]
#
## thread-caching malloc
#cc_library(
#  name = "tcmalloc",
#  visibility = ["//visibility:public"],
#  deps = select({
#    # tcmalloc is not compitable with asan/tsan/msan, so we remove it.
#    "//tools/cpp:opt_enabled": [ ":tcmalloc_opt"],
#    "//conditions:default": [":tcmalloc_debug"],
#  })
#)
#
#cc_library(
#  name = "tcmalloc_heapcheck",
#  visibility = ["//visibility:public"],
#  testonly = 1,
#  deps = select({
#    # tcmalloc is not compitable with asan/tsan/msan, so we remove it.
#    "//tools/cpp:opt_enabled": [ ":tcmalloc_opt_heapcheck"],
#    "//conditions:default": [":tcmalloc_debug_heapcheck"],
#  })
#)
#
## opt version
#cc_library(
#  name = "tcmalloc_opt",
#  srcs = [
#    "gperftools/src/tcmalloc.cc",
#  ] + MALLOC_HOOK_SRCS,
#  copts = TCMALLOC_CFLAGS + [
#    "-DNO_HEAP_CHECK",
#  ],
#  deps = [
#    ":internal",
#    ":raw_printer",
#  ],
#  alwayslink = 1,
#)
#
## tcmalloc with heap checker
#cc_library(
#  name = "tcmalloc_opt_heapcheck",
#  srcs = [
#    "gperftools/src/tcmalloc.cc",
#  ] + MALLOC_HOOK_SRCS + HEAP_CHECKER_SRCS,
#  copts = TCMALLOC_CFLAGS,
#  deps = [
#    ":internal",
#    ":thread_lister",
#    ":raw_printer",
#  ],
#  testonly = 1,
#  alwayslink = 1,
#)
#
#### ------- tcmalloc_debug (thread-caching malloc with debugallocation)
## Like tcmalloc.cc, debugallocation.cc needs exceptions to fulfill its
## API.  Luckily, we can reuse everything else from tcmalloc_minimal.
#cc_library(
#  name = "tcmalloc_debug",
#  srcs = [
#    "gperftools/src/debugallocation.cc",
#  ] +  MALLOC_HOOK_SRCS,
#  copts = TCMALLOC_CFLAGS + [
#    "-DNO_HEAP_CHECK",
#    "-DTCMALLOC_FOR_DEBUGALLOCATION",
#  ],
#  deps = [
#    ":internal",
#    ":raw_printer",
#  ],
#  alwayslink = 1,
#)
#
#cc_library(
#  name = "tcmalloc_debug_heapcheck",
#  srcs = [
#    "gperftools/src/debugallocation.cc",
#  ] + MALLOC_HOOK_SRCS + HEAP_CHECKER_SRCS,
#  copts = TCMALLOC_CFLAGS + [
#    "-DTCMALLOC_FOR_DEBUGALLOCATION",
#  ],
#  deps = [
#    ":internal",
#    ":raw_printer",
#    ":thread_lister",
#  ],
#  alwayslink = 1,
#  testonly = 1,
#)
#
## Test related stuff
## ==================
#cc_library(
#  name = "testutil",
#  copts = AM_CXXFLAGS,
#  testonly = 1,
#  srcs = [
#    "gperftools/src/tests/testutil.h",
#    "gperftools/src/tests/testutil.cc",
#  ],
#)
#
#cc_test(
#  name = "addressmap_unittest",
#  srcs = [
#    "gperftools/src/tests/addressmap_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":logging",
#  ]
#)
#
#cc_test(
#  name = "atomicops_unittest",
#  srcs = [
#    "gperftools/src/tests/atomicops_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":spinlock",
#  ]
#)
#
#cc_test(
#  name = "current_allocated_bytes_test",
#  srcs = [
#    "gperftools/src/tests/current_allocated_bytes_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#cc_test(
#  name = "debugallocation_test",
#  srcs = [
#    "gperftools/src/tests/debugallocation_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc_debug",
#  ]
#)
#
#cc_test(
#  name = "heap-checker_unittest",
#  srcs = [
#    "gperftools/src/tests/heap-checker_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc_heapcheck",
#  ],
#  linkstatic = 1,
#)
#
#sh_test(
#  name = "heap-checker_unittest_sh",
#  srcs = [
#    "runtest.sh",
#  ],
#  data = [
#    "gperftools/src/tests/heap-checker_unittest.sh",
#    "gperftools/src/pprof",
#    ":heap-checker_unittest",
#  ],
#  args = [
#    "heap-checker_unittest.sh",
#  ]
#)
#
#cc_test(
#  name = "heap-profiler_unittest",
#  srcs = [
#    "gperftools/src/tests/heap-profiler_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ],
#  linkstatic = 1,
#)
#
#sh_test(
#  name = "heap-profiler_unittest_sh",
#  srcs = [
#    "runtest.sh",
#  ],
#  data = [
#    "gperftools/src/tests/heap-profiler_unittest.sh",
#    "gperftools/src/pprof",
#    ":heap-profiler_unittest",
#  ],
#  args = [
#    "heap-profiler_unittest.sh",
#  ]
#)
#
#cc_test(
#  name = "large_heap_fragmentation_unittest",
#  srcs = [
#    "gperftools/src/tests/large_heap_fragmentation_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    # tcmalloc_debug is too slow to run this test.
#    ":tcmalloc_opt",
#  ],
#)
#
#cc_test(
#  name = "low_level_alloc_unittest",
#  srcs = [
#    "gperftools/src/tests/low_level_alloc_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "malloc_extension_c_test",
#  srcs = [
#    "gperftools/src/tests/malloc_extension_c_test.c",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    # tcmalloc_debug may perform new operation inside free function,
#    # that's not expected in this test.
#    ":tcmalloc_opt",
#  ],
#)
#
#cc_test(
#  name = "malloc_extension_test",
#  srcs = [
#    "gperftools/src/tests/malloc_extension_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "malloc_hook_test",
#  srcs = [
#    "gperftools/src/tests/malloc_hook_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "markidle_unittest",
#  srcs = [
#    "gperftools/src/tests/markidle_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "memalign_unittest",
#  srcs = [
#    "gperftools/src/tests/memalign_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "packed-cache_test",
#  srcs = [
#    "gperftools/src/tests/packed-cache_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "page_heap_test",
#  srcs = [
#    "gperftools/src/tests/page_heap_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "pagemap_unittest",
#  srcs = [
#    "gperftools/src/tests/pagemap_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "profiledata_unittest",
#  srcs = [
#    "gperftools/src/tests/profiledata_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":profiler",
#    ":tcmalloc",
#  ],
#)
#
#cc_test(
#  name = "profile-handler_unittest",
#  srcs = [
#    "gperftools/src/tests/profile-handler_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":profiler",
#    ":tcmalloc",
#  ],
#)
#
## profiler1-4 are used by profiler_unittest_sh
#cc_binary(
#  name = "profiler1_unittest",
#  srcs = [
#    "gperftools/src/tests/profiler_unittest.cc",
#  ],
#  testonly = 1,
#  copts = AM_CXXFLAGS + [
#    "-g",
#    "-DNO_THREADS",
#  ],
#  deps = [
#    ":testutil",
#    ":profiler",
#    ":tcmalloc",
#  ],
#)
#
#cc_binary(
#  name = "profiler2_unittest",
#  srcs = [
#    "gperftools/src/tests/profiler_unittest.cc",
#  ],
#  testonly = 1,
#  copts = AM_CXXFLAGS + [
#    "-g",
#    "-DNO_THREADS",
#  ],
#  deps = [
#    ":testutil",
#    ":profiler",
#    ":tcmalloc",
#  ],
#)
#
#cc_binary(
#  name = "profiler3_unittest",
#  srcs = [
#    "gperftools/src/tests/profiler_unittest.cc",
#  ],
#  testonly = 1,
#  copts = AM_CXXFLAGS + [
#    "-g",
#    "-pthread",
#  ],
#  deps = [
#    ":testutil",
#    ":profiler",
#    ":tcmalloc",
#  ],
#)
#
#cc_binary(
#  name = "profiler4_unittest",
#  srcs = [
#    "gperftools/src/tests/profiler_unittest.cc",
#  ],
#  testonly = 1,
#  copts = AM_CXXFLAGS + [
#    "-g",
#    "-pthread",
#  ],
#  deps = [
#    ":testutil",
#    ":profiler",
#    ":tcmalloc",
#  ],
#)
#
#sh_test(
#  name = "profiler_unittest_sh",
#  srcs = [
#    "runtest.sh",
#  ],
#  data = [
#    "gperftools/src/tests/profiler_unittest.sh",
#    "gperftools/src/pprof",
#    ":profiler1_unittest",
#    ":profiler2_unittest",
#    ":profiler3_unittest",
#    ":profiler4_unittest",
#  ],
#  args = [
#    "profiler_unittest.sh",
#  ],
#  tags = [
#    "manual",  # Broken
#  ],
#)
#
#cc_test(
#  name = "raw_printer_test",
#  srcs = [
#    "gperftools/src/tests/raw_printer_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#cc_test(
#  name = "realloc_unittest",
#  srcs = [
#    "gperftools/src/tests/realloc_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#cc_test(
#  name = "sampler_test",
#  srcs = [
#    "gperftools/src/tests/sampler_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#cc_binary(
#  name = "sampling_test",
#  testonly = 1,
#  srcs = [
#    "gperftools/src/tests/sampling_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#sh_test(
#  name = "sampling_test_sh",
#  srcs = [
#    "runtest.sh",
#  ],
#  data = [
#    "gperftools/src/tests/sampling_test.sh",
#    "gperftools/src/pprof",
#    ":sampling_test",
#  ],
#  args = [
#    "sampling_test.sh",
#  ]
#)
#
#cc_test(
#  name = "simple_compat_test",
#  srcs = [
#    "gperftools/src/tests/simple_compat_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#cc_test(
#  name = "stack_trace_table_test",
#  srcs = [
#    "gperftools/src/tests/stack_trace_table_test.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ]
#)
#
#cc_test(
#  name = "stacktrace_unittest",
#  srcs = [
#    "gperftools/src/tests/stacktrace_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":logging",
#    ":stacktrace",
#  ]
#)
#
#cc_test(
#  name = "system-alloc_unittest",
#  srcs = [
#    "gperftools/src/tests/system-alloc_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":tcmalloc",
#  ],
#  linkstatic = 1,
#)
#
#cc_test(
#  name = "tcmalloc_unittest",
#  srcs = [
#    "gperftools/src/tests/tcmalloc_unittest.cc",
#  ],
#  copts = ["-fno-builtin"] + AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    # tcmalloc_debug is doing something unexpected than the test(like
#    # realloc)
#    ":tcmalloc_opt",
#  ],
#  linkstatic = 1,
#)
#
#sh_test(
#  name = "tcmalloc_unittest_sh",
#  srcs = [
#    "runtest.sh",
#  ],
#  data = [
#    "gperftools/src/tests/tcmalloc_unittest.sh",
#    "gperftools/src/pprof",
#    ":tcmalloc_unittest",
#  ],
#  args = [
#    "tcmalloc_unittest.sh",
#  ]
#)
#
#cc_test(
#  name = "tcmalloc_large_unittest",
#  srcs = [
#    "gperftools/src/tests/tcmalloc_large_unittest.cc",
#  ],
#  copts = ["-fno-builtin"] + AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    ":tcmalloc",
#  ],
#  linkstatic = 1,
#)
#
#cc_test(
#  name = "thread_dealloc_unittest",
#  srcs = [
#    "gperftools/src/tests/thread_dealloc_unittest.cc",
#  ],
#  copts = AM_CXXFLAGS,
#  deps = [
#    ":testutil",
#    ":tcmalloc",
#  ]
#)
