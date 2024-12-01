cc_library(
    name = "icuuc",
    srcs = glob(["icu4c/source/common/*.cpp", "icu4c/source/common/*.h"]),
    hdrs = glob(["icu4c/source/common/unicode/*.h"]),
    includes = ["icu4c/source/common"],
    defines = ["U_COMMON_IMPLEMENTATION"],
    visibility = ["//visibility:public"],
)