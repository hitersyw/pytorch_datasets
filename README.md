# pytorch_datasets

Repo to keep datasets organized in one location.

Also for keeping loading functions for images, videos, etc.


## Installation

Install into a virtual environment for ease of use.

```
workon <virtualenv name>
cd pytorch_datasets
pip install -e .
```

## Getting Started

Once installed, can import any dataset like so:

```
import pytorch_datasets
dset = pytorch_datasets.EPFL()
print(dset.__getitem__(0))
```

## Datasets in repo

### EPFL (Multi-View Car Dataset)

- 20 sequences of cars as they rotate by 360 degrees. 2299 images total.
- [Website](https://cvlab.epfl.ch/data/data-pose-index-php/), [Paper](https://infoscience.epfl.ch/record/146798/files/multiview.pdf)

### WCVP (Weizmann Cars ViewPoint)

- Images circling around 22 cars outside. 1530 images total.
- [Website](http://www.wisdom.weizmann.ac.il/~vision/WCVP/), [Paper](http://dx.doi.org/10.1016/j.imavis.2012.09.006)

### ObjectNet3D

- 3D object locations and orientation in images. 100 object categories, 90,127 images, 201,888 objects total in these images.
- [Website](http://cvgl.stanford.edu/projects/objectnet3d/), [Paper](http://cvgl.stanford.edu/papers/xiang_eccv16.pdf)

### MISTIC-SL

- RGB videos of surgeons performing a running suture on a phantom.
- [Website](https://projects.lcsr.jhu.edu/hmm/main/index.php/DataSets/MISTIC)

### JIGSAWS

- RGB videos + kinematics of eight surgeons with different levels of skill performing five repetitions of three elementary surgical tasks on a bench-top model.
- [Website](https://cirl.lcsr.jhu.edu/research/hmm/datasets/jigsaws_release), [Paper](https://cirl.lcsr.jhu.edu/wp-content/uploads/2015/11/JIGSAWS.pdf)
