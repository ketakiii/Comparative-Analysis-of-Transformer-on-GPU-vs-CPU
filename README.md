# Comparative-Analysis-of-Transformer-on-GPU-vs-CPU


https://arxiv.org/abs/2308.06017


In machine translation tasks, the relationship between model complexity and performance is often presumed to be linear, increasing the number of parameters and consequent demands for computational resources like multiple GPUs. This study
challenges this assumption by systematically exploring the effects of hyperparameters through ablation on a sequence-to-sequence
machine translation pipeline, utilizing a single NVIDIA A100 GPU. Contrary to expectations, our experiments reveal that combinations with the most parameters were not necessarily the most effective. This unexpected insight prompted a careful reduction in
parameter sizes, uncovering ”sweet spots” that enable training sophisticated models on a single GPU without compromising translation quality. The findings demonstrate an intricate relationship between hyperparameter selection, model size, and computational
resource needs. The insights from this study contribute to the ongoing efforts to make machine translation more accessible and
cost-effective, emphasizing the importance of precise hyperparameter tuning over mere scaling. To start with the project of multiprocessing a model on GPU, we began by understanding the basics of multiprocessing. 
There are multiple ways of working with
CUDA: CUDA C/C++: a most common and flexible way to use CUDA while writing code in C/C++ 
pyCUDA: gives us complete access to CUDA C/C++ API in Python code. We would still have to write the C/C++ code in Python. 
Numba: this method does not expose the entire CUDA C/C++ API, yet allows acceleration with very less modifications while writing the code in Python itself.


https://arxiv.org/abs/2308.06017
