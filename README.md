 ### IP-Adapter
Effective and lightweight adapter to achieve image prompt capability for the pre-trained text-to-image diffusion models. An IP-Adapter with only 22M parameters can achieve comparable or even better performance to a fine-tuned image prompt model. IP-Adapter can be generalized not only to other custom models fine-tuned from the same base model, but also to controllable generation using existing controllable tools. Moreover, the image prompt can also work well with the text prompt to accomplish multimodal image generation.
# Installation
```Prompt
# install latest diffusers
pip install diffusers==0.22.1

# install ip-adapter
git clone https://github.com/Mrkomiljon/IP_adapter.git

# download the models
cd IP-Adapter
git lfs install
git clone https://huggingface.co/h94/IP-Adapter
mv IP-Adapter/models models
mv IP-Adapter/sdxl_models sdxl_models

# then you can use the notebook
```
# Download Models
you can download models from here. To run the demo, you should also download the following models:

[runwayml/stable-diffusion-v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5)

[stabilityai/sd-vae-ft-mse](https://huggingface.co/stabilityai/sd-vae-ft-mse)

[SG161222/Realistic_Vision_V4.0_noVAE](https://huggingface.co/SG161222/Realistic_Vision_V4.0_noVAE)

[ControlNet models](https://huggingface.co/lllyasviel)

# Read image prompt
![abbb](https://github.com/Mrkomiljon/IP_adapter/assets/92161283/9c6c56a0-27f5-487c-a855-f8b16013c633)

# Prompt:
```Prompt
[future car concept], no handle, lasers, holograms, [human avatars], city, no rearview mirrors, red carpet, [yellow plastic seats]
```![abbb](https://github.com/Mrkomiljon/IP_adapter/assets/92161283/9c6c56a0-27f5-487c-a855-f8b16013c633)

<p float="left">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/4f62ae7c-c240-4353-a9bf-7ea4316df6b1" width="256" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/50efb257-8250-4f8b-b7a1-9c7473c16234" width="256" />
</p>

<p float="right">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/c3437cff-6711-4a20-b6f0-10132a9be76b" width="256" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/db7db0ff-9382-4156-9176-6c396ab96bf3" width="256" />
</p>
)


