# Copyright (c) 2019 PaddlePaddle Authors. All Rights Reserved.
# 
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
# 
# http://www.apache.org/licenses/LICENSE-2.0
# 
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

add_library(nnadapter_runtime_device STATIC device.cc)
add_library(nnadapter_runtime_context STATIC context.cc)
add_library(nnadapter_runtime_model STATIC model.cc)
add_library(nnadapter_runtime_compilation STATIC compilation.cc)
add_library(nnadapter_runtime_execution STATIC execution.cc)

set(nnadapter_runtime nnadapter_runtime_device nnadapter_runtime_context nnadapter_runtime_model nnadapter_runtime_compilation nnadapter_runtime_execution CACHE INTERNAL "")
