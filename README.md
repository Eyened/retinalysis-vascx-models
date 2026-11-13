---
license: cc-by-nc-4.0
pipeline_tag: image-segmentation
tags:
- medical
- biology
- ophthalmology
- retina
---

> [!IMPORTANT]
> The entire VascX pipeline, including feature extraction is available here: [retinalysis-vascx](https://github.com/eyened/retinalysis-vascx). A new preprint presenting the pipeline is [available here](https://arxiv.org/abs/2602.08580). We will stop supporting this repository and move to the new one linked above. We will keep updating the models and pipeline there.

# 👁️ VascX models

This repository contains model weights and model cards for the VascX models from the paper [VascX Models: Model Ensembles for Retinal Vascular Analysis from Color Fundus Images](https://arxiv.org/abs/2409.16016).

The legacy `vascx_models` Python package and CLI have been removed. For inference and the complete analysis pipeline, use [retinalysis-vascx](https://github.com/eyened/retinalysis-vascx).

The model weights are in [huggingface](https://huggingface.co/Eyened/vascx).

<img src="imgs/samples_vascx_hrf.png">

## Model cards

Please see the model card for each model for details about its training procedure, datasets and ciations. For example:

- **Artery-vein** segmentation:
    - [Original version (july24)](artery_vein/av_july24.md)
    - [Updated version (may26)](artery_vein/av_may26.md)
- **Optic disc** segmentation:
    - [Original version (july24)](disc/disc_july24.md)
    - [Updated version (may26)](disc/disc_may26.md)
- **Fovea localisation**:
    - [Original version (july24)](fovea/fovea_july24.md)
    - [Updated version (may26)](fovea/fovea_may26.md)
- **Quality estimation**:
    - [Original version (july24)](quality/quality.md)
- **Vessel** segmentation:
    - [Original version (july24)](vessels/vessels_july24.md)
    - [Updated version (may26)](vessels/vessels_may26.md)

> [!IMPORTANT]
> VascX models were trained using datasets kindly made available by the ophthalmic community. The model cards above indicate which (publicly-available) datasets were used for training. We encourage VascX users to consider citing the source datasets when they are relevant to their work.

## Licensing

We share the models under a Creative Commons Attribution–NonCommercial 4.0 license. We note that some of the datasets used for training and evaluating the model ensembles were made publicly available for research purposes only. We encourage due diligence for any applications with potential for commercial use.