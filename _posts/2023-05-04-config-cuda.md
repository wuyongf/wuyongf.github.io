## [Config] CUDA

Testing

---
### Knowledge
- About cuda, pytorch, cudnn:
   - pytorch has its own version and corresponding cuda version.
   - each cuda version will also have a cudnn version.
- How to switch cuda version:
```yaml
1. install .run file: sudo sh cuda_11.8.0_520.61.05_linux.run --silent --toolkit --toolkitpath=/usr/local/cuda-11.8
2. soft link cuda-version to cuda: sudo rm cuda?  sudo ln -snf /usr/local/cuda-11.8   /usr/local/cuda
3. edit ./bashrc file: cuda-version
4. check nvcc version: nvcc -v /// nvidia-smi
```

### Version
- Config 1

```yaml
pytorch: v2.0
cuda: 12.1
cudnn:
```

- Config 2

```yaml
pytorch: v1.9.1
cuda: 11.3
cudnn: 
```