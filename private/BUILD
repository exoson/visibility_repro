load("@bazel_skylib//rules:common_settings.bzl", "bool_flag")

bool_flag(
    name = "flag",
    build_setting_default = True,
)

config_setting(
    name = "_private_config_setting",
    flag_values = {":flag": "True"},
    visibility = ["//visibility:private"],
)

alias(
    name = "alias_private_config_setting",
    actual = ":_private_config_setting",
    visibility = ["//visibility:public"],
)

