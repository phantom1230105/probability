# Copyright 2020 The TensorFlow Probability Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
# ============================================================================
# Description:
#   Functions and boilerplate for the Statistical Rethinking notebooks

package(
    # default_applicable_licenses
    default_visibility = [
        "//tensorflow_probability/examples:__subpackages__",
    ],
)

licenses(["notice"])

py_library(
    name = "rethinking",
    srcs = ["__init__.py"],
    deps = [":quap"],
)

py_library(
    name = "quap",
    srcs = ["quap.py"],
    deps = [
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_test(
    name = "quap_test",
    size = "large",
    srcs = ["quap_test.py"],
    deps = [
        ":rethinking",
        # tensorflow dep,
        "//tensorflow_probability",
        "//tensorflow_probability/python/internal:test_util",
    ],
)
