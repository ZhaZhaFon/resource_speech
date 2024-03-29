# resource_speech

## 通用 General

### 教程 Tutorials
* **Deep Learning for Human Lagnguage Processsing (DLHLP) @ National Taiwan University**
    * 李宏毅博士在国立台湾大学开的课程 Lecture by Dr. by Hung-yi Lee at National Taiwan University
    * [website@NTU](https://speech.ee.ntu.edu.tw/~hylee/dlhlp/2020-spring.php)

### 语料库 Corpus
* **WSJ0(Wall Street Journal)** 
    * 可用于语音分离、语音增强、语音识别等任务 for tasks including Speech Separation, Speech Enhancement, ASR...
    * [paper (HLT 1992)](https://dl.acm.org/doi/pdf/10.3115/1075527.1075614)
    * [LDC (官方链接 official link)](https://catalog.ldc.upenn.edu/LDC93S6A)
* **LibriSpeech**
    * 可用于语音识别等任务 for tasks including ASR, Speech Separation, Speech Enhancement...
    * [paper (ICASSP 2015)](https://www.danielpovey.com/files/2015_icassp_librispeech.pdf)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/12/)
* **AISHELL-1**
    * 可用于语音识别、说话人识别等任务 for tasks including ASR, Speaker Recognition...
    * [paper (COCOSDA 2017)](https://ieeexplore.ieee.org/document/8384449)
    * [website@aishelltech (官方链接 official link)](http://www.aishelltech.com/kysjcp)

### 数据增强 Data Augmentation
* **RIR_NOISES**
    * 房间冲击响应(RIR)数据, 可用于语音识别、说话人识别中的数据增强 Room Impulse Response(RIR) data for data augmentation in ASR, Speaker Recognition...
    * [paper (ICASSP 2017)](https://ieeexplore.ieee.org/abstract/document/7953152)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/28/)
* **MUSAN**
    * 包含音乐、语音、噪声三类录音, 可用于语音识别、说话人识别中的数据增强 MUsic, Speech And Noise recordings for data augmentation in ASR, Speaker Recognition...
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/17/)

### 活动音检测(VAD) Voice Activity Detection
* **SileroVAD**
    * [GitHub (官方代码 official code)](https://github.com/snakers4/silero-vad)
    * [Torch Hub (预训练模型 pretrained models)](https://pytorch.org/hub/snakers4_silero-vad_vad/)
* **py-webrtcvad**
    * [GitHub (官方代码 official code)](https://github.com/wiseman/py-webrtcvad)

### 多用途开发工具箱 General-purpose Development Toolkits
* **SpeechBrain**
    * 基于PyTorch的通用语音工具包, 支持语音识别、语音前端、说话人识别、情感识别、关键词识别、口语理解等多种语音任务和数据集 Development toolkits for multiple speech tasks including ASR, Speech Front-end, Speaker Recognition, Keyword Spotting, Spoken Language Understanding... and corresponding recipes, built upon PyTorch.
    * [paper (arXiv 2021)](https://arxiv.org/abs/2106.04624)
    * [GitHub (代码仓库 code repository)](https://github.com/speechbrain/speechbrain)
    * [Doc (官方文档 official documentations)](https://speechbrain.readthedocs.io/en/latest/index.html)

### 语音工具 Speech Tools
* **FFmpeg**
    * [官方文档 official documentations](https://ffmpeg.org/documentation.html)
* **SoX**
    * [官方文档 official documentations](http://sox.sourceforge.net/Docs/Documentation)

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

### 语音前端 - 代码 Codebase
* **Asteroid Toolkits**
    * 基于PyTorch Lightning的深度学习语音前端工具包, 支持语音增强/语音分离/多模态/多通道等语音前端任务和数据集 Toolkits for deep-learning-based speech front-end development, built upon PyTorch Lightning, suports for various recipes and tasks including Speech Enhancement, Speech Separation, Multi-modal, Mulit-channel...
    * [paper (INTERSPEECH 2020)](http://www.interspeech2020.org/uploadfile/pdf/Wed-2-4-4.pdf)
    * [GitHub (代码仓库 code repository)](https://github.com/asteroid-team/asteroid)
    * [Doc (官方文档 official documentations)](https://asteroid-team.github.io/asteroid/why_use_asteroid.html)
* **Google / VoiceFilter**
    * 基于dvector说话人表征和的CNN-LSTM分离网络的目标说话人提取 Target Speaker Extraction based on dvector speaker embedding and CNN-LSTM separation network
    * [paper (INTERSPEECH 2019)](https://arxiv.org/abs/1810.04826) & [paper (INTERSPEECH 2020)](https://arxiv.org/abs/2009.04323)
    * [GitHub (作者推荐的非官方复现 non-official re-implementation recommended by the authors)](https://github.com/mindslab-ai/voicefilter)
* **BUTSpeechFIT / SpeakerBeam**
    * 基于Asteroid的TD-SpeakerBeam官方复现 Official re-implementation of TD-SpeakerBeam based on Asteroid toolkits
    * [paper (ICASSP 2020)](https://ieeexplore.ieee.org/abstract/document/9054683)
    * [GitHub (BUT官方开源代码 official code released BUT)](https://github.com/BUTSpeechFIT/speakerbeam)

## 说话人识别(SR) Speaker Recognition

### 说话人识别 - SOTA
* **VoxSRC-20 track 1**
    * 说话人识别竞赛, 只能用VoxCeleb数据, 在VoxCeleb上进行评测 Speaker Recognition competition evaluated on VoxCeleb, only VoxCeleb can be used
    * [website@VoxSRC-20 (竞赛官网 challenge website)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/competition2020.html)
    * [Leaderboard](https://competitions.codalab.org/competitions/26120)
* **VoxSRC-20 track 2**
    * 说话人识别竞赛, 无数据约束, 在VoxCeleb上进行评测 Speaker Recognition competition evaluated on VoxCeleb, no limitation on data
    * [website@VoxSRC-20 (竞赛官网 challenge website)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/competition2020.html)
    * [Leaderboard](https://competitions.codalab.org/competitions/34066#results)

### 说话人识别 - 数据集
* **VoxCeleb1**
    * 可用于说话人验证、说话人辨认等任务 for tasks including Speaker Verification, Speaker Identification...
    * [paper (INTERSPEECH 2017)](https://arxiv.53yu.com/abs/1706.08612)
    * [website@VGG-Oxford (官方链接 official link)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox1.html)
    * [website@Graviti](https://gas.graviti.cn/dataset/hello-dataset/VoxCeleb1/download)
* **VoxCeleb2**
    * 可用于说话人验证、说话人辨认等任务 for tasks including Speaker Verification, Speaker Identification...
    * [paper (INTERSPEECH 2018)](https://arxiv.53yu.com/abs/1806.05622)
    * [website@VGG-Oxford (官方链接 official link)](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox2.html)
    * [website@Graviti](https://gas.graviti.cn/dataset/hello-dataset/VoxCeleb2/download)
* **CN-Celeb1**
    * 可用于说话人验证、说话人辨认、说话人检索等任务 for tasks including Speaker Verification, Speaker Identification, Speaker Retrieval...
    * [paper (ICASSP 2020)](http://128.84.21.203/abs/1911.01799)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/82/)
* **CN-Celeb2**
    * 可用于说话人验证、说话人辨认、说话人检索等任务 for tasks including Speaker Verification, Speaker Identification, Speaker Retrieval...
    * [paper (Speech Communication 2022)](http://128.84.4.34/abs/2012.12468)
    * [OpenSLR (官方链接 official link)](https://www.openslr.org/82/)

### 说话人识别 - 代码 Codebase
* **THU-CSLT / Sunine**
    * 支持VoxCeleb、CN-Celeb等数据集, 支持TDNN、ResNetSE34、ECAPA-TDNN等网络 Support various recipes(VoxCeleb/CN-Celeb) and network architectures(TDNN/ResNet34/ECAPA-TDNN)
    * [GitLab (THU-CSLT开发的代码库 codebase developed by THU-CSLT)](https://gitlab.com/csltstu/sunine))
* **clovaai / voxceleb_trainer**
    * 支持VoxCeleb, 支持VGGVox、ResNetSE34等网络, 支持多分类、度量学习等训练方式 Support VoxCeleb, support networks including VGGVox and ResNetSE34, support training methods including multi-class classification and metric learning
    * [paper (INTERSPEECH 2020)](https://arxiv.org/abs/2003.11982)
    * [GitHub (Oxford-VGG开发的代码库 codebase developed by Oxford-VGG)](https://github.com/clovaai/voxceleb_trainer)

## 说话人分割(SD) Speaker Diarization 

### 说话人分割 - Awesome
* **wq2012/awesome-diarization**
    * [wq2012/awesome-diarization](https://github.com/wq2012/awesome-diarization#Clustering)

### 说话人分割 - SOTA
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
* **wq2012 / SpectralCluster**
    * 基于谱聚类的说话人分割 Speaker Diarization based on spectral clustering
    * [paper (ICASSP 2018)](https://google.github.io/speaker-id/publications/LstmDiarization/)
    * [GitHub (Google的官方程序 official code in GitHub from Google)](https://github.com/wq2012/SpectralCluster)
* **BUTSpeechFIT / VBx**
    * 基于变分贝叶斯-的说话人分割聚类 Speaker Diarization based on variational Bayes HMM
    * [paper (Computer Speech & Language)](https://www.sciencedirect.com/science/article/pii/S0885230821000619)
    * [GitHub (BUT开发的代码库 codebase developed by BUT-SpeechFIT)](https://github.com/BUTSpeechFIT/VBx/tree/master)

### 说话人分割 - 评测 Evaluation
* **VoxSRC-20 Evaluation Toolkits**
    * 包括DER、JER等指标 metrics including DER, JER...
    * [GitHub (VoxSRC-20的官方程序 official code from VoxSRC-20)](https://github.com/a-nagrani/VoxSRC2020)

## 音频标注(AT) Audio Tagging 

### 音频标注 - 数据集 Dataset
* **FSDKaggle2018**
    * 可用于音频标注、声源分离等任务 for tasks including Audio Tagging, general Sound Source Separation...
    * [Zenodo (官方链接 Official Link)](https://zenodo.org/record/2552860#.YnS_OPNByjC)

## 语音预训练(PTM) Pre-Training for Speech

### 语音预训练 - 代码 Codebase
* **S3PRL toolkits**
    * 语音预训练和SUPERB基准工具包 Toolkits for Pre-Training in Speech and the SUPERB benchmark
    * [GitHub (官方代码)](https://github.com/s3prl/s3prl)

## 关键词识别(KWS) Keyword Spotting

## 语音合成(TTS) Text-To-Speech

### 语音合成 - 教程 Tutorials
* **cnlinxi / book-text-to-speech**
    * 一个比较全面的TTS概览性教程 A comprehensive TTS tutorial
    * [GitHub](https://github.com/cnlinxi/book-text-to-speech)

### 语音合成 - 代码 Codebase
* **jaywalnut310 / vits**
    * Kakao官方开源的VITS代码(1阶段端到端TTS) Official code by Kakao Enterprise for VITS, a one-stage end-to-end TTS model
    * [paper (ICML 2021)](https://arxiv.org/abs/2106.06103)
    * [GitHub (Kakao的官方开源代码 official code released by Kakao Enterprise)](https://github.com/jaywalnut310/vits)
