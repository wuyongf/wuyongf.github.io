## [Config] CUDA

Testing

---
### Knowledge
- About cuda, pytorch, cudnn:
   - pytorch has its own version and corresponding cuda version.
   - each cuda version will also have a cudnn version.
- How to switch cuda version
    - install .run file: `sudo sh cuda_11.8.0_520.61.05_linux.run --silent --toolkit --toolkitpath=/usr/local/cuda-11.8`
  - soft link cuda-version to cuda: 
    - cuda-12.1 `sudo ln -snf /usr/local/cuda-12.1   /usr/local/cuda`
    - cuda-11.8 `sudo ln -snf /usr/local/cuda-11.8   /usr/local/cuda`
    - cuda-11.3 `sudo ln -snf /usr/local/cuda-11.3   /usr/local/cuda`
  - edit ./bashrc file: `gedit ~/.bashrc` and `source ~/.bashrc`
  - check nvcc/cuda version: `nvcc --version` and `nvidia-smi`

### Version
- Config 1
  ```yaml
  nvidia driver: latest
  pytorch: 2.0.0
  cuda: 12.1
  cudnn:
  gcc: `latest version. 11.3` 
  ```

- Config 2 - Working
  ```yaml
  nvidia driver: latest
  pytorch: 2.0.0
  cuda: 11.8
  cudnn: 
  gcc: `latest version. 11.3` 
  ```

- Config 2
  ```yaml
  pytorch: v1.9.1
  cuda: 11.3
  cudnn: 
  gcc: 9
  ```

### myPC congif
#### GCC 
  - Version: 12, 11, 9
  - How to switch GCC version: [csdn](https://blog.csdn.net/wanggao_1990/article/details/120989070)
  - set priority:`sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-11 100 --slave /usr/bin/g++ g++ /usr/bin/g++-11 --slave /usr/bin/gcov gcov /usr/bin/gcov-11`
  - to switch gcc: `sudo update-alternatives --config gcc`
  - to check gcc version: `which gcc && gcc --version`

#### CUDA
  - to install: `sudo sh cuda_11.3.0_465.19.01_linux.run --silent --toolkit --toolkitpath=/usr/local/cuda-11.3`
  - to soft link cuda: 
    - cuda-12.1 `sudo ln -snf /usr/local/cuda-12.1   /usr/local/cuda`
    - cuda-11.8 `sudo ln -snf /usr/local/cuda-11.8   /usr/local/cuda`
    - cuda-11.3 `sudo ln -snf /usr/local/cuda-11.3   /usr/local/cuda`
  - to edit `~/.bashrc` file: `gedit ~/.bashrc` and `source ~/.bashrc`
  - to check nvcc/cuda version: `nvcc --version` and `nvidia-smi`

####
pip install mmcv-full -f https://download.openmmlab.com/mmcv/dist/cu113/torch2.0.0/index.html
#### temp
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-11 80 --slave /usr/bin/g++ g++ /usr/bin/g++-11 --slave /usr/bin/gcov gcov /usr/bin/gcov-11
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-9 70 --slave /usr/bin/g++ g++ /usr/bin/g++-9 --slave /usr/bin/gcov gcov /usr/bin/gcov-9 

- switch gcc
- switch cuda soft link
- edit `~/.bashrc`  