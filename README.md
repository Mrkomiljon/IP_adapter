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

# Only image prompt
<div align="center">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/f04c96c8-485c-47bf-9711-08417fb7aa74" width="400" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/dedf3df7-7867-493f-81f4-1eb0ea4e2bc3" width="400" />
</div>

<div align="center">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/2ed51b54-8671-4796-b59b-85759ea71f1f" width="400" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/0f0199b9-9fd3-42c1-8455-680963d635ce" width="400" />
</div>

# Prompt:
```Prompt
[future car concept], no handle, lasers, holograms, [human avatars], city, no rearview mirrors, red carpet, [yellow plastic seats]
```

<div align="center">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/4f62ae7c-c240-4353-a9bf-7ea4316df6b1" width="400" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/50efb257-8250-4f8b-b7a1-9c7473c16234" width="400" />
</div>

<div align="center">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/c3437cff-6711-4a20-b6f0-10132a9be76b" width="400" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/db7db0ff-9382-4156-9176-6c396ab96bf3" width="400" />
</div>

# Prompt

```Prompt
Generate an image of a futuristic Hyundai car model 10 years into the future, With the iconic 'H' symbol prominent and recognizable in the steering wheel',
negative_prompt = monochrome, lowres, bad anatomy, worst quality, low quality
```
<div align="center">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/51bc86fb-3c46-4f34-a493-29e2a83ffdce" width="400" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/daba2f9b-9917-4d54-8d8e-4dda1da465eb" width="400" />
</div>

<div align="center">
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/b802602c-e213-4efa-a3c2-d8846d271cbf" width="400" />
  <img src="https://github.com/Mrkomiljon/IP_adapter/assets/92161283/21300d9a-20ab-45c2-917d-6a769f1a53af" width="400" />
</div>



