licenses(["notice"])

cc_library(
  name = "gmock",
  testonly = 1,
  visibility = ["//visibility:public"],
  includes = [
    "gmock-1.7.0/include",
  ],
  srcs = [
    'gmock-1.7.0/src/gmock-all.cc',
  ],
  hdrs = glob([
    'gmock-1.7.0/include/**/*.h',
    'gmock-1.7.0/src/*.h',
    'gmock-1.7.0/src/*.cc',
  ]),
  deps = [
    "//external:gtest",
  ],
  copts = [
    '-iquotegooglemock/gmock-1.7.0'
  ]
)

cc_library(
  name = "gmock_main",
  testonly = 1,
  visibility = ["//visibility:public"],
  deps = [
    ":gmock",
  ],
  srcs = [
    "gmock-1.7.0/src/gmock_main.cc",
  ],
)
