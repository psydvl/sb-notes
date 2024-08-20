#GPU #openSUSE #AMD #ROCM

# Drivers
https://www.amd.com/en/support/download/linux-drivers.html
https://amdgpu-install.readthedocs.io/en/latest/
No openSUSE Slowroll/Tumbleweed -> selected rhel 9.4

`sudo rpm -i *.rpm --test`

## Drivers
https://repo.radeon.com/amdgpu/6.1.3/rhel/9.4/main/x86_64/
amdgpu-lib
vulkan-amdgpu

## ROCM
https://repo.radeon.com/rocm/rhel9/6.1.3/main/
rocm-hip-runtime
rocm-opencl-runtime

# PyTorch
[[Notes/PyTorch#ROCM]]

# ROCM
```bash
export HSA_OVERRIDE_GFX_VERSION=11.0.0
export TORCH_BLAS_PREFER_HIPBLASLT=0
python3 Fooocus/entry_with_update.py --disable-xformers --always-cpu --attention-split
```