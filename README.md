# SimpleITK Python Notebooks

As of this writing, SimpleITK version >=1.0.0 is required to run these notebooks. This version is available from [PyPi](https://pypi.python.org/pypi/SimpleITK) and [Source Forge](http://sourceforge.net/projects/simpleitk/files/SimpleITK/1.0.0/Python/).

## Setting Up a Python Environment

我们建议您设置一个单独的Python虚拟环境来运行这些notebook作为教程。

## Anaconda
使用[Anaconda](https://www.continuum.io/) 您可以设置名为sitkpy的虚拟环境，并使用1个命令安装包括SimpleITK在内的所有依赖项:

    conda env create -f environment.yml


## Plain Python

安装 virtualenv并创建名为sitkpy的环境。

    sudo pip install virtualenv
    virtualenv ~/sitkpy --no-site-packages

安装所有必需的软件包和SimpleITK，并激活ipywidgets笔记本扩展。

    ~/sitkpy/bin/pip install -r Python/requirements.txt
    jupyter nbextension enable --py --sys-prefix widgetsnbextension

The requirements.txt file just lists the required packages ([see](requirements.txt)).


### Downloading Data

执行笔记本时，数据会自动下载到“Data”目录。

或者，事先下载所有数据：

    cd SimpleITK-Notebooks
    Utilities/downloaddata.py Data/ Data/manifest.json

### Run the notebooks

To launch:

    cd SimpleITK-Notebooks/Python
    ~/sitkpy/bin/jupyter notebook

### Working offline

在某些情况下，例如教程会话，您可能无法访问Internet。这要求你：

1. 事先下载所有数据 - 见上面。

# View Static Converted Pages

- [00 Setup](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/00_Setup.html)
- [01 Image Basics](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/01_Image_Basics.html)
- [02 Pythonic Image](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/02_Pythonic_Image.html)
- [03 Image Details](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/03_Image_Details.html)
- [10 matplotlib's imshow](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/10_matplotlib's_imshow.html)
- [20 Expand With Interpolators](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/20_Expand_With_Interpolators.html)
- [21 Transforms and Resampling](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/21_Transforms_and_Resampling.html)
- [22 Transforms](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/22_Transforms.html)
- [300 Segmentation Overview](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/300_Segmentation_Overview.html)
- [30 Segmentation Region Growing](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/30_Segmentation_Region_Growing.html)
- [31 Levelset Segmentation](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/31_Levelset_Segmentation.html)
- [32 Watersheds Segmentation](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/32_Watersheds_Segmentation.html)
- [33 Segmentation Thresholding Edge Detection](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/33_Segmentation_Thresholding_Edge_Detection.html)
- [34 Segmentation Evaluation](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/34_Segmentation_Evaluation.html)
- [41 Progress](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/41_Progress.html)
- [51 VH Segmentation1](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/51_VH_Segmentation1.html)
- [55 VH Resample](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/55_VH_Resample.html)
- [56 VH Registration1](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/56_VH_Registration1.html)
- [60 Registration Introduction](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/60_Registration_Introduction.html)
- [61 Registration Introduction Continued](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/61_Registration_Introduction_Continued.html)
- [62 Registration Tuning](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/62_Registration_Tuning.html)
- [63 Registration Initialization](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/63_Registration_Initialization.html)
- [64 Registration Memory Time Tradeoff](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/64_Registration_Memory_Time_Tradeoff.html)
- [65 Registration FFD](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/65_Registration_FFD.html)
- [66 Registration Demons](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/66_Registration_Demons.html)
- [67 Registration Semiautomatic Homework](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/67_Registration_Semiautomatic_Homework.html)
