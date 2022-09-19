# RePaint
**Inpainting using Denoising Diffusion Probabilistic Models**



This repository was created by Giulia Neccia e Luca Gaudenzi for the Neural Networks exam.
This git was cloned from https://github.com/andreas128/RePaint
## Setup

### 1. Code

```bash
git clone https://github.com/andreas128/RePaint.git
```

### 2. Environment
```bash
pip install numpy torch blobfile tqdm pyYaml pillow    # e.g. torch 1.7.1+cu110.
```

### 3. Download models and data

```bash
pip install --upgrade gdown && bash ./download.sh
```

That downloads the models for ImageNet, CelebA-HQ, and Places2, as well as the face example and example masks.


### 4. Run example
```bash
python test.py --conf_path confs/face_example.yml
```
Find the output in `./log/face_example/inpainted`






## Details on data

**Which datasets and masks have a ready-to-use config file?**

We provide config files for ImageNet (inet256), CelebA-HQ (c256) and Places2 (p256) for the masks "thin", "thick", "every second line", "super-resolution", "expand" and "half" in [`./confs`](https://github.com/andreas128/RePaint/tree/main/confs). You can use them as shown in the example above.

**Details on performed tests**
In the directory ./out_test there are configuration files for some tests that have been performed (in particular that on our paper) and in ./out_test/Results there are the output images.





# Acknowledgement



This repository is based on [RePaint](https://github.com/andreas128/RePaint).
