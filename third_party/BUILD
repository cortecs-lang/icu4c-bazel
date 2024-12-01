cc_library(
    name = "stubdata",
    srcs = glob([
        "icu4c/source/stubdata/*.cpp",
        "icu4c/source/stubdata/*.h",
    ]),
    visibility = ["//visibility:public"],
    deps = [":icuuc_headers"],
)

cc_library(
    name = "icuuc_headers",
    srcs = glob([
        "icu4c/source/common/*.h",
    ]),
    hdrs = glob(["icu4c/source/common/unicode/*.h"]),
    includes = ["icu4c/source/common"],
)

cc_library(
    name = "icuuc",
    srcs = glob([
        "icu4c/source/common/*.cpp",
    ]),
    defines = ["U_COMMON_IMPLEMENTATION"],
    visibility = ["//visibility:public"],
    deps = [
        ":icuuc_headers",
        ":stubdata",
    ],
)

cc_library(
    name = "icui18n",
    srcs = glob([
        "icu4c/source/i18n/*.cpp",
        "icu4c/source/i18n/*.h",
    ]),
    hdrs = glob(["icu4c/source/i18n/unicode/*.h"]),
    defines = ["U_I18N_IMPLEMENTATION"],
    includes = ["icu4c/source/i18n"],
    visibility = ["//visibility:public"],
    deps = [":icuuc"],
)
