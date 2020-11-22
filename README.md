# Detectron2 Tutorial
A brief introductory tutorial to the [Detectron2](https://github.com/facebookresearch/detectron2) library.

For more information, refer to the [blog post](TBD).

By Sebastian Castro, 2020

---

# Getting Started

First, you will need a Linux or macOS environment set up with Python 3.6 or higher.

* Create a fresh virtual environment, e.g., `python3 -m venv .virtualenvs/detectron2`
* Activate the virtual environment, e.g., `source .virtualenvs/detectron2/bin/activate`
* `pip install wheel`
* `pip install jupyter torch torchvision`

* Install Detectron2 as outlined in [the Detectron2 install guide](https://github.com/facebookresearch/detectron2/blob/master/INSTALL.md). For Torch 1.7 / CUDA 11.0 (which is what I have used for developing this tutorial)
```
python -m pip install detectron2 -f \
  https://dl.fbaipublicfiles.com/detectron2/wheels/cu110/torch1.7/index.html
```

* Set up OpenCV. Detectron2 requires Python 3.6 or higher so you will have to install from source according to this resource: 
https://docs.opencv.org/master/d2/de6/tutorial_py_setup_in_ubuntu.html

---

# Labeling Data

We have used [coco-annotator](https://github.com/jsbroks/coco-annotator) to manually label our data and export it to the popular COCO data format.

This repository includes a small dataset so you can try Detectron2 without having to collect and label your own data.

---

# Using Detectron2 for Object Detection

Once your environment is set up, you can follow along the notebooks in this repository.

* [`detectron_pretrained.ipynb`](detection2_pretrained.ipynb) shows how to use pretrained models from the Detectron2 Model Zoo.
* [`detection_tutorial.ipynb`](detectron2_tutorial.ipynb) shows how to train a model on a custom dataset by starting from one of the pretrained models above.

