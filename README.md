# gem5_nvmain_memory_project

## 環境
Ubuntu 64-bit 18.04 - VMware workstation 16 player
p.s. 
* 20.04的g++太新，nvmain不支援
* gem5不支援Ubuntu 16.04

## get started
* 安裝一些工具如git、m4、python等等
ˋˋˋ
sudo apt install build-essential git m4 scons zlib1g zlib1g-dev libprotobuf-dev protobuf-compiler libprotoc-dev libgoogle-perftools-dev python3-dev python3-six python libboost-all-dev pkg-config
ˋˋˋ
* 測試HELLO WORLD，可以由gem5/m5out中的stat.txt查看cache hit 的次數
ˋˋˋ ./build/X86/gem5.opt configs/example/se.py -c tests/test-progs/hello/bin/x86/linux/hello --cpu-type=TimingSimpleCPU --caches --l2cache --mem-type=NVMainMemory --nvmain-config=../NVmain/Config/PCM_ISSCC_2012_4GB.configˋˋˋ
