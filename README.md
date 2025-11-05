<div align="center">

<h1>SuperCLIP</h1>
<p>Official codebase for SuperCLIP.</p>

</div>

---

## Table of Contents
- [News](#news)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Datasets](#datasets)
  - [Configuration](#configuration)
- [Training](#training)
- [Acknowledgments](#acknowledgments)

## News

- 2025-09-19: Accepted by NeurIPS 2025. [✔]
- 2025-11-06: Code release. [✔]

## Getting Started

### Installation

```bash
# Clone the repository
git clone https://github.com/hustvl/SuperCLIP.git
cd SuperCLIP

# Install dependencies
pip install -r requirements.txt
```

### Datasets

- Datacomp-1B: https://github.com/mlfoundations/datacomp
- ImageNet-1K: https://www.image-net.org/download.php

### Configuration

Update the paths in the training script to point to your local datasets:
- Set DATA_PATH to the Datacomp-1B root.
- Set VAL_DATA_PATH to the ImageNet-1K validation set.

File to edit: train.sh

## Training

Start SuperCLIP training with:

```bash
bash train.sh <config_path> superclip
```

## Acknowledgments

Our codebase is built upon:
- OpenCLIP: https://github.com/mlfoundations/open_clip
- SuperClass: https://github.com/x-cls/superclass?tab=readme-ov-file

We thank the OpenCLIP and SuperClass teams for contributing such impressive code and models to the community.