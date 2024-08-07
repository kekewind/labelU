<div align="center">
<article style="display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <p align="center"><img width="300" src="https://user-images.githubusercontent.com/25022954/209616423-9ab056be-5d62-4eeb-b91d-3b20f64cfcf8.svg" /></p>
    <h1 style="width: 100%; text-align: center;"></h1>
    <p align="center">
        English | <a href="./README_zh-CN.md" >简体中文</a>
    </p>
</article>
    
   
</div>

## Product Introduction

LabelU is a comprehensive data annotation platform designed for handling multimodal data. It offers a range of advanced annotation tools and efficient workflows, making it easier for users to tackle annotation tasks involving images, videos, and audio. LabelU is tailored to meet the demands of complex data analysis and model training.

## Key Features

### Versatile Image Annotation Tools
LabelU provides a robust set of image annotation tools, including 2D bounding boxes, semantic segmentation, polylines, and keypoints. These tools are adaptable to a wide range of image processing tasks, enabling users to efficiently complete image labeling, annotation, and analysis.

### Powerful Video Annotation Capabilities
For video annotation, LabelU offers strong processing capabilities, supporting video segmentation, video classification, and video information extraction. Users can easily manage long-duration videos and extract key information, providing high-quality annotated data for subsequent model training.

### Efficient Audio Annotation Tools
LabelU also features powerful audio annotation tools with efficient and precise audio analysis capabilities. These tools support audio segmentation, audio classification, and audio information extraction. By visualizing complex sound information, LabelU simplifies the audio data processing workflow, facilitating more accurate model development.


## Features

- Simplicity: Provides a variety of image annotation tools that can be annotated through simple visual configuration.
- Flexibility: A variety of tools can be freely combined to meet most image, video, and audio annotation needs.
- Universality: Supports exporting to various data formats, including JSON, COCO, MASK.

## Getting started

- <a href="https://opendatalab.github.io/labelU-Kit/">
    <button>Try LabelU annotation toolkit</button>
</a>

- <a href="https://labelu.shlab.tech/">
    <button>Try LabelU online</button>
</a>

### Local deployment

1. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html), Choose the corresponding operating system type and download it for installation.

> **Note：** If your system is MacOS with an Intel chip, please install [Miniconda of intel x86_64](https://repo.anaconda.com/miniconda/)。

2. After the installation is complete, run the following command in the terminal (you can choose the default 'y' for prompts during the process):

```bash
conda create -n labelu python=3.11
```

> **Note：** For Windows platform, you can run the above command in Anaconda Prompt.

3. Activate the environment：

```bash
conda activate labelu
```

4. Install LabelU：

```bash
pip install labelu
```

> To install the test version：`pip install --extra-index-url https://test.pypi.org/simple/ labelu==<test revision>`

5. Run LabelU：

```bash
labelu
```

6. Visit [http://localhost:8000/](http://localhost:8000/) and ready to go.

### Local development

```bash
# Download and Install miniconda
# https://docs.conda.io/en/latest/miniconda.html

# Create virtual environment(python = 3.11)
conda create -n labelu python=3.11

# Activate virtual environment
conda activate labelu

# Install peotry
# https://python-poetry.org/docs/#installing-with-the-official-installer

# Install all package dependencies
poetry install

# Start labelu, server: http://localhost:8000
uvicorn labelu.main:app --reload

# Update submodule
git submodule update --remote --merge
```

## Supported Scenarios

### Image

- Label Classification: Can help users quickly classify objects in images and can be used for image retrieval, object detection tasks.
- Text Description: Text transcription can help users quickly extract text information in images and can be used for text retrieval, machine translation tasks.
- Bounding Box: Can help users quickly select objects in images and can be used for image recognition, object tracking tasks.
- Point Annotation: Points can help users accurately label key information in the image and can be used for object recognition, scene analysis tasks.
- Polygon: Can help users accurately label irregular shapes and can be used for object recognition, scene analysis tasks.
- Line Annotation: Lines can help users accurately label edges and contours in the image and can be used for object recognition, scene analysis tasks.
- Cuboid: Cuboid can help users accurately label the size, shape, and location of objects within images, and can be used for object recognition, scene analysis tasks.

### Video

- Label Classification: Classifying and labeling videos can be used for video retrieval, recommendation, and classification tasks.
- Text Description: Converting speech content in videos into text can be used for voice recognition, transcription, and translation tasks.
- Segment Segmentation: Extracting specific clips or scenes from the video for annotation is very useful for video object detection, action recognition, and video summary tasks.
- Timestamps: Point to or mark specific parts of the video; users can click on timestamps to jump directly to that part of the video.

### Audio

- Label Classification: By listening to the audio and selecting the appropriate classification for annotation, it's applicable for audio retrieval, recommendations, and classification tasks.
- Text Description: Converting speech content in audio into text makes it easier for users to analyze and process text. It's very useful for voice recognition, transcription tasks, and can help users better understand and process voice content.
- Segment Segmentation: Extracting specific clips from audio for annotation is very useful for audio event detection, voice recognition, and audio editing tasks.
- Timestamps: Used to point to or mark specific parts of the audio; users can click on timestamps to jump directly to that part of the audio.

## Quick start

- [Guidance](https://opendatalab.github.io/labelU)

## Annotation format

- [Documentation](https://opendatalab.github.io/labelU/#/schema)

## Citation

```bibtex
@article{he2024opendatalab,
  title={Opendatalab: Empowering general artificial intelligence with open datasets},
  author={He, Conghui and Li, Wei and Jin, Zhenjiang and Xu, Chao and Wang, Bin and Lin, Dahua},
  journal={arXiv preprint arXiv:2407.13773},
  year={2024}
}
```

## Communication

Welcome to the OpenDataLab official WeChat group！

<p align="center">
<img style="width: 400px" src="https://user-images.githubusercontent.com/25022954/208374419-2dffb701-321a-4091-944d-5d913de79a15.jpg">
</p>


## Links

- [LabelU-kit](https://github.com/opendatalab/labelU-Kit) Web front-end annotation kit (LabelU is based on this JavaScript kit)
- [LabelLLM](https://github.com/opendatalab/LabelLLM) An Open-source LLM Dialogue Annotation Platform
- [Miner U](https://github.com/opendatalab/MinerU) A One-stop Open-source High-quality Data Extraction Tool

## License

This project is released under the [Apache 2.0 license](./LICENSE).
