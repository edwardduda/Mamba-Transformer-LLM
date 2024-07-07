This repo is a hobby project where I explore the usage of the Mamba architecture used in conjunction with transformers for training LLMs. 
The Mamba architecture is a selective state space mechanism that using convolutions to create a sort of self-attention mechanism found in transformers.
Mamba blocks are advantageous because they require less parameters to function saving memory, have a linear time complexity, and when used with transformers, offer equivalent performance. 


## Acknowledgements

This project uses code from the following repositories:

1. **build-nanogpt** by Andrej Karpathy (https://github.com/karpathy)
    - Repository URL: [https://github.com/karpathy/build-nanogpt]
    - License: MIT
2. **mamba** by Tri Dao, Albert Gu (https://github.com/state-spaces)
    - Repository URL: [https://github.com/state-spaces/mamba]
    - License: Apache

## Setup - Local Conda
    ```bash
    git clone git@github.com:edwardduda/Mamba-Transformer-LLM.git
    conda create -y --name Mamba-Transformer-LLM python=3.12
    conda activate Mamba-Transformer-LLM
    pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
    pip install tiktoken==0.7.0
    pip install datasets==2.20.0
    cd Mamba-Transformer-LLM
    git clone https://github.com/state-spaces/mamba.git
    pip install packaging==24.1
    pip install causal-conv1d>=1.2.0
    cd mamba && pip install -e . && cd ..
    pip install wandb==0.17.1
    ```
## Setup - Docker


-README.me
    This file.

