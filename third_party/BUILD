cc_library(
    name = "icuuc",
    srcs = glob(["icu4c/source/common/*.cpp", "icu4c/source/common/*.h"]),
    hdrs = glob(["icu4c/source/common/unicode/*.h"]),
    includes = ["icu4c/source/common"],
    defines = ["U_COMMON_IMPLEMENTATION"],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "icui18n",
    srcs = glob(["icu4c/source/i18n/*.cpp", "icu4c/source/i18n/*.h"]),
    hdrs = glob(["icu4c/source/i18n/unicode/*.h"]),
    includes = ["icu4c/source/i18n"],
    defines = ["U_I18N_IMPLEMENTATION"],
    deps = [":icuuc"],
    visibility = ["//visibility:public"],
)