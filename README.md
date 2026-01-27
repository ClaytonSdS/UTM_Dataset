<img src="https://github.com/ClaytonSdS/VisionGauge/blob/main/steps/utm_dataset_logo2.png?raw=true" width="900"/>


# **Dataset Description**

This dataset was created to support Article X and is available on [Roboflow](https://universe.roboflow.com/visiongauge/utm_dataset-ooorv) and [Hugging Face](https://huggingface.co/datasets/claytonsds/UTM_Dataset).

It consists of images of **U-tube manometers** constructed using a **transparent PVC water level hose (5/16" × 1 mm)** and **flexible measuring tapes of different colors**, each with a length of **150 cm (60 inches)**. The manometric fluids represented in the dataset include **water, oil, and dyed water**. The dataset is intended for **computer vision regression and classification tasks**, specifically targeting the **reading of liquid column levels**.

The dataset includes **48,218 augmented images**, derived from **20,036 unique original images**. All annotations were performed using the RoboFlow Annotate Tool, with label precision within ± 0.1 cm.


# **Dataset Split**
![dataset distribution](https://github.com/ClaytonSdS/VisionGauge/blob/main/steps/dataset_distribution_hf.png?raw=true)

* **Training set:** 42274 images
* **Validation set:** 5319 images
* **Test set:** 625 images

# Data Structure

The dataset follows a standard split structure:
```
dataset/
├── train/
│   ├── 10.2/
│   │   ├── image23.png
│   │   └── ...
│   ├── 10.4/
│   └── ...
├── validation/
│   ├── 9.8/
│   └── ...
└── test/
│    ├── 10.0/
│    └── ...
└── dataset_mapping.csv
```

* Each subfolder name corresponds to the **label value** (e.g., water column height in centimeters).
* Images inside the folder share the same height value.

---

# License

This dataset is released under the **Apache License 2.0**.

---


# **Citation**

```bibtex
@dataset{utm_dataset,
	author    = {Santos, Clayton Silva},
	title     = {{UTM} {Dataset}},
	year      = {2026},
	month     = {jan},
	publisher = {Roboflow},
	version   = {27},
	doi       = {10.5281/zenodo.18259826},
	url       = {https://universe.roboflow.com/visiongauge/utm_dataset-ooorv}
}
```
