#AMD #AI #GPU #generation #ROCM

# Install
```sh
git clone https://github.com/lllyasviel/Fooocus.git
cd Fooocus
python3 -m venv venv
source venv/bin/activate
pip install -r requirements_versions.txt
```
# PyTorch
## ROCM
[[Notes/AMDGPU#PyTorch]]


# Script
```bash
#!/usr/bin/env bash
cd Fooocus
source venv/bin/activate
export HSA_OVERRIDE_GFX_VERSION=11.0.0
export TORCH_BLAS_PREFER_HIPBLASLT=0
python3 entry_with_update.py --disable-xformers --always-cpu --attention-split
#python3 entry_with_update.py --disable-xformers --always-gpu --attention-split
```