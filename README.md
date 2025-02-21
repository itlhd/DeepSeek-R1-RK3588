Extract the files from the compressed file to the development board, and then run deepseek according to the following command：
```
root@armsom:/mnt# cp demo_Linux_aarch64 /userdata/
root@armsom:/mnt# cp DeepSeek-R1-Distill-Qwen-1.5B_W8A8_RK3588.rkllm /userdata/demo_Linux_aarch64
export LD_LIBRARY_PATH=./lib
taskset f0 ./llm_demo ./DeepSeek-R1-Distill-Qwen-1.5B_W8A8_RK3588.rkllm  2048 4096
```
For more information, please refer to the [RKLM toolchain](https://github.com/airockchip/rknn-llm/tree/main) released by rockchip
