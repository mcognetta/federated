package(default_visibility = ["//tensorflow_federated:__subpackages__"])

licenses(["notice"])  # Apache 2.0

py_library(
    name = "emnist",
    srcs = ["__init__.py"],
)

py_library(
    name = "models",
    srcs = ["models.py"],
    srcs_version = "PY3",
)

py_binary(
    name = "run_experiment",
    srcs = ["run_experiment.py"],
    python_version = "PY3",
    srcs_version = "PY3",
    deps = [
        ":models",
        "//tensorflow_federated",
        "//tensorflow_federated/python/research/utils",
        "//tensorflow_federated/python/research/utils:training_loops",
    ],
)
