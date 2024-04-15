# Comparing `tmp/tinyrl-0.3.0.tar.gz` & `tmp/tinyrl-0.3.1.tar.gz`

## Comparing `tinyrl-0.3.0.tar` & `tinyrl-0.3.1.tar`

### file list

```diff
@@ -1,294 +1,294 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/__init__.py
--rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers.h
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/version.h
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
--rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
--rw-r--r--   0        0        0    35055 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
--rw-r--r--   0        0        0    25276 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
--rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
--rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
--rw-r--r--   0        0        0    19878 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
--rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
--rw-r--r--   0        0        0    34738 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
--rw-r--r--   0        0        0    21772 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
--rw-r--r--   0        0        0     8459 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
--rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
--rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
--rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
--rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
--rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/algorithms/ppo/ppo.h
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/algorithms/sac/default.h
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/algorithms/sac/template.h
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/inference/inference.cpp
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/python_environment/operations_cpu.h
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/python_environment/python_environment.h
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/interface/training/training.cpp
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/accelerate.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/compile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/link_accelerate.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/link_mkl.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/load_checkpoint.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/load_module.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/render.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 tinyrl-0.3.0/tinyrl/src/sac.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tinyrl-0.3.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.3.0/LICENSE
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 tinyrl-0.3.0/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tinyrl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 tinyrl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/__init__.py
+-rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers.h
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/version.h
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
+-rw-r--r--   0        0        0    35055 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    25276 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
+-rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
+-rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
+-rw-r--r--   0        0        0    19878 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
+-rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
+-rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
+-rw-r--r--   0        0        0    34738 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
+-rw-r--r--   0        0        0    21772 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
+-rw-r--r--   0        0        0     8459 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
+-rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
+-rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
+-rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
+-rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
+-rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
+-rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
+-rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/algorithms/ppo/ppo.h
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/algorithms/sac/default.h
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/algorithms/sac/template.h
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/inference/inference.cpp
+-rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/python_environment/operations_cpu.h
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/python_environment/python_environment.h
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/training/training.cpp
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/__init__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/accelerate.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/compile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/link_accelerate.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/link_mkl.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/load_checkpoint.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/load_module.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/render.py
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/sac.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tinyrl-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 tinyrl-0.3.1/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tinyrl-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 tinyrl-0.3.1/PKG-INFO
```

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/version.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/version.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/persist/code.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/persist/code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,23 @@
             static constexpr TI CRITIC_NUM_LAYERS = 3;
             static constexpr auto CRITIC_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
 
             static constexpr TI EPISODE_STEP_LIMIT = 1000;
             static constexpr TI N_ENVIRONMENTS = 64;
             static constexpr TI ON_POLICY_RUNNER_STEPS_PER_ENV = 64;
             static constexpr TI BATCH_SIZE = ON_POLICY_RUNNER_STEPS_PER_ENV * N_ENVIRONMENTS;
+
+            using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
         };
 
         template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
         struct ConfigApproximatorsMLP{
             using ACTOR_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::BATCH_SIZE>;
-            using ACTOR_OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI>;
-            using CRITIC_OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI>;
+            using ACTOR_OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
+            using CRITIC_OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
             using ACTOR_OPTIMIZER = nn::optimizers::Adam<ACTOR_OPTIMIZER_SPEC>;
             using CRITIC_OPTIMIZER = nn::optimizers::Adam<CRITIC_OPTIMIZER_SPEC>;
             using ACTOR_SPEC = nn_models::mlp::AdamSpecification<ACTOR_STRUCTURE_SPEC>;
             using ACTOR_TYPE = nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<ACTOR_SPEC>;
             using ACTOR_TYPE_INFERENCE = nn_models::mlp_unconditional_stddev::NeuralNetwork<ACTOR_SPEC>;
             using CRITIC_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::BATCH_SIZE>;
             using CRITIC_SPEC = nn_models::mlp::AdamSpecification<CRITIC_STRUCTURE_SPEC>;
```

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         static constexpr auto ACTOR_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
         static constexpr TI CRITIC_HIDDEN_DIM = 64;
         static constexpr TI CRITIC_NUM_LAYERS = 3;
         static constexpr auto CRITIC_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
 
         static constexpr bool COLLECT_EPISODE_STATS = true;
         static constexpr TI EPISODE_STATS_BUFFER_SIZE = 1000;
+
+        using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
     };
 
     // The approximator config sets up any types that support the usual rl_tools::forward and rl_tools::backward operations (can be custom as well)
     // We provide approximators based on the sequential and mlp models. The latter (mlp) allows for a variable number of layers, but is restricted to a uniform hidden layer size while the former allows for arbitrary layers to be combined in a sequential manner. Both support compile-time autodiff
     template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS, typename CONTAINER_TYPE_TAG>
     struct ConfigApproximatorsSequential{
         template <typename PARAMETER_TYPE, template<typename> class LAYER_TYPE = nn::layers::dense::LayerBackwardGradient>
@@ -66,29 +68,29 @@
             using LAYER_2 = LAYER_TYPE<LAYER_2_SPEC>;
             using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, 1, nn::activation_functions::ActivationFunction::IDENTITY, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Output, CONTAINER_TYPE_TAG>;
             using LAYER_3 = LAYER_TYPE<LAYER_3_SPEC>;
 
             using MODEL = Module<LAYER_1, Module<LAYER_2, Module<LAYER_3>>>;
         };
 
-        using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI>;
+        using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
 
         using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
 
         using ACTOR_TYPE = typename ACTOR<nn::parameters::Adam>::MODEL;
         using CRITIC_TYPE = typename CRITIC<nn::parameters::Adam>::MODEL;
         using CRITIC_TARGET_TYPE = typename CRITIC<nn::parameters::Plain, nn::layers::dense::Layer>::MODEL;
     };
 
     template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS, typename T_CONTAINER_TYPE_TAG>
     struct ConfigApproximatorsMLP{
         using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
         using ACTOR_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, 2*ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::TANH, PARAMETERS::SAC_PARAMETERS::ACTOR_BATCH_SIZE, CONTAINER_TYPE_TAG>;
         using CRITIC_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE, CONTAINER_TYPE_TAG>;
-        using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI>;
+        using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
         using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
         using ACTOR_SPEC = nn_models::mlp::AdamSpecification<ACTOR_STRUCTURE_SPEC>;
         using ACTOR_TYPE = nn_models::mlp::NeuralNetworkAdam<ACTOR_SPEC>;
 
         using CRITIC_SPEC = nn_models::mlp::AdamSpecification<CRITIC_STRUCTURE_SPEC>;
         using CRITIC_TYPE = nn_models::mlp::NeuralNetworkAdam<CRITIC_SPEC>;
```

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         static constexpr auto ACTOR_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
         static constexpr TI CRITIC_HIDDEN_DIM = 64;
         static constexpr TI CRITIC_NUM_LAYERS = 3;
         static constexpr auto CRITIC_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
 
         static constexpr bool COLLECT_EPISODE_STATS = true;
         static constexpr TI EPISODE_STATS_BUFFER_SIZE = 1000;
+
+        using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
     };
 
     // The approximator config sets up any types that support the usual rl_tools::forward and rl_tools::backward operations (can be custom as well)
     // We provide approximators based on the sequential and mlp models. The latter (mlp) allows for a variable number of layers, but is restricted to a uniform hidden layer size while the former allows for arbitrary layers to be combined in a sequential manner. Both support compile-time autodiff
     template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
     struct ConfigApproximatorsSequential{
         template <typename PARAMETER_TYPE, template<typename> class LAYER_TYPE = nn::layers::dense::LayerBackwardGradient>
@@ -66,29 +68,29 @@
             using LAYER_2 = LAYER_TYPE<LAYER_2_SPEC>;
             using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, 1, nn::activation_functions::ActivationFunction::IDENTITY, PARAMETER_TYPE, BATCH_SIZE>;
             using LAYER_3 = LAYER_TYPE<LAYER_3_SPEC>;
 
             using MODEL = Module<LAYER_1, Module<LAYER_2, Module<LAYER_3>>>;
         };
 
-        using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI>;
+        using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
 
         using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
 
         using ACTOR_TYPE = typename ACTOR<nn::parameters::Adam>::MODEL;
         using ACTOR_TARGET_TYPE = typename ACTOR<nn::parameters::Adam, nn::layers::dense::Layer>::MODEL;
         using CRITIC_TYPE = typename CRITIC<nn::parameters::Adam>::MODEL;
         using CRITIC_TARGET_TYPE = typename CRITIC<nn::parameters::Adam, nn::layers::dense::Layer>::MODEL;
     };
 
     template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
     struct ConfigApproximatorsMLP{
         using ACTOR_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::TANH, PARAMETERS::TD3_PARAMETERS::ACTOR_BATCH_SIZE>;
         using CRITIC_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::TD3_PARAMETERS::CRITIC_BATCH_SIZE>;
-        using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI>;
+        using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
         using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
         using ACTOR_SPEC = nn_models::mlp::AdamSpecification<ACTOR_STRUCTURE_SPEC >;
         using ACTOR_TYPE = nn_models::mlp::NeuralNetworkAdam<ACTOR_SPEC>;
 
         using ACTOR_TARGET_SPEC = nn_models::mlp::InferenceSpecification<ACTOR_STRUCTURE_SPEC>;
         using ACTOR_TARGET_TYPE = nn_models::mlp::NeuralNetwork<ACTOR_TARGET_SPEC>;
```

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h` & `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/interface/algorithms/ppo/ppo.h` & `tinyrl-0.3.1/tinyrl/interface/algorithms/ppo/ppo.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/interface/algorithms/sac/default.h` & `tinyrl-0.3.1/tinyrl/interface/algorithms/sac/default.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/interface/algorithms/sac/template.h` & `tinyrl-0.3.1/tinyrl/interface/algorithms/sac/template.h`

 * *Files 12% similar despite different names*

```diff
@@ -35,11 +35,17 @@
     static constexpr TI ACTOR_NUM_LAYERS = $ACTOR_NUM_LAYERS;
     static constexpr auto ACTOR_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$ACTOR_ACTIVATION_FUNCTION;
     static constexpr TI CRITIC_HIDDEN_DIM = $CRITIC_HIDDEN_DIM;
     static constexpr TI CRITIC_NUM_LAYERS = $CRITIC_NUM_LAYERS;
     static constexpr auto CRITIC_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$CRITIC_ACTIVATION_FUNCTION;
     static constexpr bool COLLECT_EPISODE_STATS = $COLLECT_EPISODE_STATS;
     static constexpr TI EPISODE_STATS_BUFFER_SIZE = $EPISODE_STATS_BUFFER_SIZE;
+    struct OPTIMIZER_PARAMETERS: rlt::nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>{
+        static constexpr T ALPHA = $OPTIMIZER_ALPHA;
+        static constexpr T BETA_1 = $OPTIMIZER_BETA_1;
+        static constexpr T BETA_2 = $OPTIMIZER_BETA_2;
+        static constexpr T EPSILON = $OPTIMIZER_EPSILON;
+    };
 };
 
 template <typename T, typename TI, typename RNG, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
 using LOOP_CORE_CONFIG_FACTORY = rlt::rl::algorithms::sac::loop::core::Config<T, TI, RNG, ENVIRONMENT, SAC_LOOP_CORE_PARAMETERS<T, TI, ENVIRONMENT, T_EPISODE_STEP_LIMIT>>;
```

### Comparing `tinyrl-0.3.0/tinyrl/interface/inference/inference.cpp` & `tinyrl-0.3.1/tinyrl/interface/inference/inference.cpp`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/interface/python_environment/python_environment.h` & `tinyrl-0.3.1/tinyrl/interface/python_environment/python_environment.h`

 * *Files 19% similar despite different names*

```diff
@@ -28,8 +28,10 @@
     using T = typename SPEC::T;
     using TI = typename SPEC::TI;
     using State = PythonEnvironmentState<T, TI, SPEC::OBSERVATION_DIM>;
     static constexpr TI OBSERVATION_DIM = SPEC::OBSERVATION_DIM;
     static constexpr TI OBSERVATION_DIM_PRIVILEGED = SPEC::OBSERVATION_DIM;
     static constexpr TI ACTION_DIM = SPEC::ACTION_DIM;
     pybind11::object* environment;
+    T action_space_range[ACTION_DIM];
+    T action_space_offset[ACTION_DIM];
 };
```

### Comparing `tinyrl-0.3.0/tinyrl/interface/training/training.cpp` & `tinyrl-0.3.1/tinyrl/interface/training/training.cpp`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/src/compile.py` & `tinyrl-0.3.1/tinyrl/src/compile.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     optimization_flag = ('-O3' if not sys.platform.startswith('win') else '/O2') if enable_optimization else ''
     arch_flag = '-march=native' if not sys.platform.startswith('win') else '/arch:AVX2'
     link_math_flag = '-lm' if not sys.platform.startswith('win') else ''
     fast_math_flag = '-ffast-math' if not sys.platform.startswith('win') else '/fp:fast'
     lto_flag = '' #'-flto' if not sys.platform.startswith('win') else '/GL'
     pic_flag = '-fPIC' if not sys.platform.startswith('win') else '/LD'
     link_stdlib_flag = '-stdlib=libc++' if sys.platform == 'darwin' else ''
+    verbose_flag = '-DTINYRL_VERBOSE' if verbose or "TINYRL_VERBOSE" in os.environ else ''
 
     # pybind_includes = subprocess.check_output(["python3", "-m", "pybind11", "--includes"]).decode().strip().split()
     pybind_includes = [f"-I{pybind11.get_include()}"]
     python_includes = ["-I" + sysconfig.get_paths()['include']] #subprocess.check_output(["python3-config", "--includes"]).decode().strip().split()
     rl_tools_includes = ["-I" + str(os.path.join(absolute_path, "..", "external", "rl_tools", "include"))]
 
     link_python_args = []
@@ -56,14 +57,15 @@
             pic_flag,
             cpp_std_flag,
             optimization_flag,
             arch_flag,
             link_math_flag,
             fast_math_flag,
             link_stdlib_flag,
+            verbose_flag,
             lto_flag,
             *flags,
             *link_python_args,
             *pybind_includes,
             *python_includes,
             *rl_tools_includes,
             source,
```

### Comparing `tinyrl-0.3.0/tinyrl/src/link_mkl.py` & `tinyrl-0.3.1/tinyrl/src/link_mkl.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/src/load_checkpoint.py` & `tinyrl-0.3.1/tinyrl/src/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/src/render.py` & `tinyrl-0.3.1/tinyrl/src/render.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/tinyrl/src/sac.py` & `tinyrl-0.3.1/tinyrl/src/sac.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,20 @@
     ACTOR_HIDDEN_DIM = 64,
     ACTOR_NUM_LAYERS = 3,
     ACTOR_ACTIVATION_FUNCTION = "RELU",
     CRITIC_HIDDEN_DIM = 64,
     CRITIC_NUM_LAYERS = 3,
     CRITIC_ACTIVATION_FUNCTION = "RELU",
     COLLECT_EPISODE_STATS = True,
-    EPISODE_STATS_BUFFER_SIZE = 1000
+    EPISODE_STATS_BUFFER_SIZE = 1000,
+    # optimizer
+    OPTIMIZER_ALPHA=1e-3,
+    OPTIMIZER_BETA_1=0.9,
+    OPTIMIZER_BETA_2=0.999,
+    OPTIMIZER_EPSILON=1e-7,
     ):
 
     use_python_environment = type(env_factory) != dict
     custom_environment_header_search_path = None if use_python_environment else env_factory["path"]
     custom_environment_flag = '-I' + custom_environment_header_search_path if custom_environment_header_search_path is not None else ''
 
     if use_python_environment:
```

### Comparing `tinyrl-0.3.0/LICENSE` & `tinyrl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/README.md` & `tinyrl-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.0/pyproject.toml` & `tinyrl-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyrl"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Jonas Eschmann", email="jonas.eschmann@gmail.com" },
 ]
 description = "A Python wrapper for RLtools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tinyrl-0.3.0/PKG-INFO` & `tinyrl-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyrl
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for RLtools
 Project-URL: Homepage, https://github.com/rl-tools/tinyrl
 Project-URL: Issues, https://github.com/rl-tools/tinyrl/issues
 Author-email: Jonas Eschmann <jonas.eschmann@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

