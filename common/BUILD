package(default_visibility = ["//visibility:public"])

cc_library(
    name = "defs",
    hdrs = ["defs.h"],
)

cc_library(
    name = "errors",
    srcs = [
        "error_strings.h",
        "errors.c",
        "errors.h",
    ],
    hdrs = ["errors.h"],
)

cc_library(
    name = "stdint",
    hdrs = ["stdint.h"],
)

cc_library(
    name = "interop",
    srcs = [
        "//common/curl-p:curl_p.c",
        "//common/curl-p:digest.c",
        "//common/model:transaction.c",
        "//common/trinary:flex_trit.c",
        "//common/trinary:trit_byte.c",
        "//common/trinary:trit_long.c",
        "//common/trinary:trit_tryte.c",
    ],
    hdrs = [
        "defs.h",
        "//common/curl-p:digest.h",
        "//common/curl-p:trit.h",
        "//common/model:transaction.h",
        "//common/trinary:bytes.h",
        "//common/trinary:flex_trit.h",
        "//common/trinary:trit_byte.h",
        "//common/trinary:trit_long.h",
        "//common/trinary:trit_tryte.h",
    ],
    defines = ["FLEX_TRIT_ENCODING_5_TRITS_PER_BYTE"],
    deps = [
        "//common:stdint",
        "//common/curl-p:trit",
        "//common/trinary:bytes",
        "//common/trinary:trits",
        "//common/trinary:tryte",
        "//utils:macros",
    ],
)
