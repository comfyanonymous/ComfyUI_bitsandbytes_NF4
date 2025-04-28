#### ~~NOTE: This is very likely Deprecated in favor of GGUF which seems to give better results~~ 
Some users can experience speedup by combining loading UNET as NF4 using the loader from this repo and load T5XXL as GGUF using the repo from https://github.com/city96/ComfyUI-GGUF

Now on the [manager](https://github.com/ltdrdata/ComfyUI-Manager) for easy installation. Make sure to select Channel:dev in the ComfyUI manager menu or install via git url.

You can find the checkpoints and UNET in the linked repositories on huggingface or by searching for NF4 on Civitai

### [CivitAI search link](https://civitai.com/search/models?baseModel=Flux.1%20S&baseModel=Flux.1%20D&sortBy=models_v9&query=nf4)

### [nf4 flux unet only](https://huggingface.co/silveroxides/flux1-nf4-unet)

### [nf4 flux dev checkpoint](https://huggingface.co/lllyasviel/flux1-dev-bnb-nf4/blob/main/flux1-dev-bnb-nf4.safetensors)

### [nf4 flux schnell checkpoint](https://huggingface.co/silveroxides/flux1-nf4-weights/blob/main/flux1-schnell-bnb-nf4.safetensors)

Requires installing bitsandbytes.

Make sure your ComfyUI is updated.

The nodes are: 
#### "CheckpointLoaderNF4": "Load NF4 Flux Checkpoint"

#### "UNETLoaderNF4": "Load NF4 Flux UNET"

just plug it in your flux workflow instead of the regular ones.

Code adapted from the implementation by Illyasviel at [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge).
