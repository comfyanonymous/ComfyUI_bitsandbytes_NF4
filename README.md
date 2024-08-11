A quickly written custom node that uses code from [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) to support the [nf4 flux checkpoints](https://huggingface.co/lllyasviel/flux1-dev-bnb-nf4/blob/main/flux1-dev-bnb-nf4.safetensors).

Requires installing bitsandbytes.

The node is: CheckpointLoaderNF4, just plug it in your flux workflow instead of the regular one.
