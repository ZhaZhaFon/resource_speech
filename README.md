# resource_speech

## 通用 General

### 语料库 Corpus

* **WSJ0**: Wall Street Journal
    * 可用于语音分离、语音增强、语音识别等任务 for tasks including Speech Separation, Speech Enhancement, ASR...
    * [paper (HLT 1992)](https://dl.acm.org/doi/pdf/10.3115/1075527.1075614)
    * [LDC (官方链接 official link)](https://catalog.ldc.upenn.edu/LDC93S6A)
* **LibriSpeech**
    * 可用于语音识别等任务 for tasks including ASR, Speech Separation, Speech Enhancement...
    * [paper (ICASSP 2015)](https://www.danielpovey.com/files/2015_icassp_librispeech.pdf)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/12/)
* **RIR_NOISES**
    * 房间冲击响应(RIR)数据, 可用于语音识别、说话人识别中的数据增强 Room Impulse Response(RIR) data for data augmentation in ASR, Speaker Recognition...
    * [paper (ICASSP 2017)](https://ieeexplore.ieee.org/abstract/document/7953152)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/28/)

## 语音前端 Speech Front-end

### 语音前端 - 数据集 Dataset
* **wsj0-2mix**
    * 可用于语音分离、语音增强等任务 for tasks including Speech Separation, Speech Enhancement...
    * [paper (ICASSP 2016)](https://arxiv.org/abs/1508.04306)
    * [台湾大学李宏毅博士上传的部分数据 some data released by Dr. Hung-yi Lee @ NTU](https://docs.google.com/presentation/d/1lskmHkti5tJjRvrl03mhuh_aMwfGA4M2Heayk5hL054/edit#slide=id.g80fe64a690_0_75)
    * [website@MERL (MERL的数据生成官方脚本 official data generation scripts from MERL)](https://www.merl.com/demos/deep-clustering)
* **LibriMix**
    * 可用于语音分离、语音增强等任务 for tasks including Speech Separation, Speech Enhancement... 
    * [paper (arXiv 2020)](https://arxiv.org/abs/2005.11262)
    * [GitHub (Inria的数据生成官方脚本 official data generation scripts from Inria](https://github.com/JorisCos/LibriMix)
* **WHAM!**
    * 噪声数据, 可用于语音增强、有噪语音分离等任务(配合wsj0-2mix、LibriMix中的语音数据) noise data for tasks including Speech Enhancement, Speech Separation under noisy environment...(normally used with speech audio from wsj0-2mix or LibriMix)
    * [paper (INTERSPEECH 2019)](https://arxiv.org/abs/1907.01160)
    * [website@Whisper.ai (官方链接 official link)](https://wham.whisper.ai/)

## 说话人识别 Speaker Recognition

### 说话人识别 - 数据集
* **VoxCeleb1**
    * 可用于说话人验证、说话人辨认等任务 for tasks including Speaker Verification, Speaker Identification...
    * [paper (INTERSPEECH 2017)](https://arxiv.53yu.com/abs/1706.08612)
    * [website@VGG-Oxford (官方链接 official link)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox1.html)
    * [website@Graviti](https://gas.graviti.cn/dataset/hello-dataset/VoxCeleb1/download)
* **VoxCeleb1**
    * 可用于说话人验证、说话人辨认等任务 for tasks including Speaker Verification, Speaker Identification...
    * [paper (INTERSPEECH 2018)](https://arxiv.53yu.com/abs/1806.05622)
    * [website@VGG-Oxford (官方链接 official link)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox2.html)
    * [website@Graviti](https://gas.graviti.cn/dataset/hello-dataset/VoxCeleb2/download)

## 说话人分割 Speaker Diarization

### 说话人分割 - Awesome
* **wq2012/awesome-diarization**
    * [wq2012/awesome-diarization](https://github.com/wq2012/awesome-diarization#Clustering)

### 说话人分割 - 基准 Benchmark
* **VoxSRC-20 track 4**
    * 说话人分割竞赛, 无数据约束, 在VoxConverse上进行评测 Speaker Diariaztion competition evaluated on VoxConverse, no limitation on data
    * [website@VoxSRC-20 (竞赛官网 challenge website)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/competition2020.html)
    * [Leaderboard](https://competitions.codalab.org/competitions/26357#results) 

### 说话人分割 - 数据集 Dataset
* **VoxConverse**
    * 可用于说话人分割相关任务 for speaker diarization and related tasks...
    * [paper (INTERSPEECH 2020)](https://arxiv.org/abs/2007.01216)
    * [website@VGG-Oxford (官方链接 official link)](https://www.robots.ox.ac.uk/~vgg/data/voxconverse/index.html)
    * [GitHub (VGG-Oxford的标签数据 ground-truth labels from VGG-Oxford)](https://github.com/joonson/voxconverse)

### 说话人分割 - 代码 Codebase
* **Spectral Clustering for Speaker Diariazation**
    * [paper (ICASSP 2018)](https://google.github.io/speaker-id/publications/LstmDiarization/)
    * [GitHub (Google的官方程序 official code in GitHub from Google)](https://github.com/wq2012/SpectralCluster)

### 说话人分割 - 评测 Evaluation
* **VoxSRC-20 Evaluation Toolkits**
    * 包括DER、JER等指标 metrics including DER, JER...
    * [GitHub (VoxSRC-20的官方程序 official code from VoxSRC-20)](https://github.com/a-nagrani/VoxSRC2020)
