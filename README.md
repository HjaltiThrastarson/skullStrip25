# skullStrip25
Contains a wrapper to execute a skull stripping method, designed for T1-weighthed MRIs and highlighted in [this](https://arxiv.org/abs/2602.08764) paper.

## Usage

The wrapper is designed for easy use, and is tested on both linux and windows operating sytems. Usage requires docker to be installed, as well as python (tested on version >3.12). The wrapper can be used as follows:

```cmd
python wrapper /path/to/input/image.nii.gz /path/to/output/ 1
```
Where the first argument is the path to the input, the second argument is the path for the output image and the third argument is for what model to use, where 1 is the larger and more accurate model, and 0 is the smaller, alternative model. In most cases the larger model is recommended, but running both might be useful for comparison and error detection. 