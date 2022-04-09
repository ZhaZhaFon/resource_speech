# resource_speech

## 通用 General

### 语料库 Corpus

* **WSJ0**: Wall Street Journal
    * 可用于语音分离、语音增强、语音识别等任务 for tasks including speech separation, speech enhancement, ASR...
    * [paper (HLT 1992)](https://dl.acm.org/doi/pdf/10.3115/1075527.1075614)
    * [LDC (官方链接 official link)](https://catalog.ldc.upenn.edu/LDC93S6A)
* **LibriSpeech**
    * 可用于语音识别等任务 for tasks including ASR, speech separation, speech enhancement...
    * [paper (ICASSP 2015)](https://www.danielpovey.com/files/2015_icassp_librispeech.pdf)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/12/)

## 语音前端 Speech Front-end

### 语音前端 - 数据集 Dataset
* **wsj0-2mix**
    * 可用于语音分离、语音增强等任务 for tasks including speech separation, speech enhancement...
    * [paper (ICASSP 2016)](https://arxiv.org/abs/1508.04306)
    * [台湾大学李宏毅博士上传的部分数据 some data released by Dr. Hung-yi Lee @ NTU](https://docs.google.com/presentation/d/1lskmHkti5tJjRvrl03mhuh_aMwfGA4M2Heayk5hL054/edit#slide=id.g80fe64a690_0_75)
* **LibriMix**
    * 可用于语音分离、语音增强等任务 for tasks including speech separation, speech enhancement... 
    * [paper (arXiv 2020)](https://arxiv.org/abs/2005.11262)
    * [GitHub (Inria的数据生成官方脚本 official data generation scripts from Inria](https://github.com/JorisCos/LibriMix)
* **WHAM!**
    * 噪声数据, 可用于语音增强、有噪语音分离等任务(配合wsj0-2mix、LibriMix中的语音数据) noise data for tasks including speech enhancement, speech separation under noisy environment...(normally used with speech audio from wsj0-2mix or LibriMix)
    * [paper (INTERSPEECH 2019)](https://arxiv.org/abs/1907.01160)
    * [website@Whisper.ai (官方链接 official link)](https://wham.whisper.ai/)

## 说话人分割 Speaker Diarization

### 说话人分割 - 基准 Benchmark
* **VoxSRC-20 track 4**
    * 说话人分割竞赛, 无数据约束, 在VoxConverse上进行评测 Speaker Diariaztion competition evaluated on VoxConverse, no limitation on data
    * [竞赛结果 Leaderboard](https://competitions.codalab.org/competitions/26357#results) 

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


