# About intel-gpu-ocl-icd-system

Home: https://github.com/IntelPython/intel-gpu-ocl-icd-feedstock

Package license: Apache 2

Feedstock license: Apache 2

Summary: Symlink system-wide OpenCL ICD file for Intel(R) GPUs to current environment

Since GPU drivers are installed system-wide, and the OpenCL loader in conda environment
is configured to look for ICD files in ``${CONDA_PREFIX}/etc/OpenCL/vendors`` to isolate
the conda environment from the system environment, enabling discovery of Intel GPU devices
by the OpenCL loader requires creation of appropriate ICD file in the conda environment's
own vendors folder. This metapackage creates such an ICD as a symbolic link to the ICD
installed system-wide.
