# AI-VIS

AI-VIS is a Conditional GAN (cGAN) based model that simulates visible imagery from multiple IR channels of geostationary weather satellites at night.

The model is trained and tested on Himawari-8/9 Full Disk and Target Area data, and we has been tested on other modern satellites including GOES-R series and GK-2A.

This repository will provide codes for the model architecture, training, and testing.

# What's new on AI-VIS 2.0

TODO

# License

License for this repo is **Apache 2.0**.

Additional terms: All images generated using AI-VIS that are made publicly available must be marked as AI-VIS generated to avoid confusion with real visible imagery.

# Citation

AI-VIS 1.0 Paper: [Simulating Nighttime Visible Satellite Imagery of Tropical Cyclones Using Conditional Generative Adversarial Networks](https://ieeexplore.ieee.org/document/10988561)

```bibtex
@ARTICLE{10988561,
  author={Yao, Jinghuai and Du, Puyuan and Zhao, Yucheng and Wang, Yubo},
  journal={IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing}, 
  title={Simulating Nighttime Visible Satellite Imagery of Tropical Cyclones Using Conditional Generative Adversarial Networks}, 
  year={2025},
  volume={18},
  number={},
  pages={12616-12633},
  keywords={Clouds;Monitoring;Cloud computing;Data models;Tropical cyclones;Spatial resolution;Satellites;Satellite broadcasting;Loss measurement;Earth;Advanced Himawari imager (AHI);clouds;conditional generative adversarial network (CGAN);deep learning;nighttime;tropical cyclone (TC);visible (VIS)},
  doi={10.1109/JSTARS.2025.3567074}}
```

# Models List of AI-VIS

| Model Name | Params* | Training Finish Time | Weights |
|------------|--------|---------------------| -------|
| aivis-1.0  |  67M   | 2024/3 | [HF🤗](https://huggingface.co/Dapiya/aivis-1.0) |
| aivis-1.5-small  |  67M   | 2024/9 | [Request form](https://docs.google.com/forms/d/1dBqFUJSB15ZhTCaj-W_WARUyOnBhL5cQANw7tEZhgeo) |
| aivis-1.5-large  |  263M   | 2024/12 | [Request form](https://docs.google.com/forms/d/1dBqFUJSB15ZhTCaj-W_WARUyOnBhL5cQANw7tEZhgeo) |
| aivis-2.0  |  TODO   | TODO | TODO |

*Params are counting the generator only, as only the generator is used during inference, and the discriminator is very small compared to the generator.
