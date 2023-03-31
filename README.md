# Music source separation literatures

|Paper|Data|Features/Input|Models|Measures|
|:--:|:--:|:--:|:--:|:--:|
|[M. Spiertz and V. Gnann (2009)](https://www.ient.rwth-aachen.de/cms/dafx09/)|EBU speech, [Instruments Data](https://link.springer.com/book/10.1007/978-0-387-21603-4)|Spectrogram, MFCC|MFCC K-means, NMF|SAR, SDR, SIR, SER|
|[G. Mysore, P. Smaragdis, and B. Raj (2010)](https://link.springer.com/chapter/10.1007/978-3-642-15995-4_18)|[TIMIT speech](https://catalog.ldc.upenn.edu/LDC93s1)|Spectrogram|Non-negative Factorial HMM|SAR, SDR, SIR|
|[R. Jaiswal, *et, al.* (2011)](https://ieeexplore.ieee.org/abstract/document/5946386)|[Orchestral Instruments](https://www.worldcat.org/ko/title/peter-siedlaczeks-advanced-orchestra-upgrade-97/oclc/43566640)|Spectrogram|Shifted-NMF|SAR, SDR, SIR|
|[E. Grais, M.U. Sen, and H. Erdogan (2014)](https://ieeexplore.ieee.org/abstract/document/6854299)|[TIMIT speech](https://catalog.ldc.upenn.edu/LDC93s1), Piano data|Spectrogram|DNN, Energy Minimization|SNR, SDR, SIR|
|[J. Le Roux, *et al.* (2015)](https://ieeexplore.ieee.org/abstract/document/7177933)|WSJ-0(speech)|Spectrogram|DeepNMF|SDR, SNR|
|[S. Uhlich, F. Giron, and Y. Mitsufuji (2015)](https://ieeexplore.ieee.org/abstract/document/7178348)|[TRIOS](https://zenodo.org/record/6797837#.Y_h6ZnZByUk) ("Brahms","Lussier")|Spectrogram|DNN(FNN)|SAR, SDR, SIR|
|[A.A. Nugraha, A. Liutkus, and E. Vincent (2016)](https://ieeexplore.ieee.org/abstract/document/7760548)|SISEC 2015 dataset|Spectrogram|DNN + Wiener filter|SAR, SDR, SIR, ISR|
|[A. Jansson, *et al.* (2017)](https://openaccess.city.ac.uk/id/eprint/19289/)|Train: Large (original, instrumental) songs , Test:iKala, MedleyDB|Spectrogram|U-Net|SAR, NSDR, SIR|
|[P. Chandna, *et al.* (2017)](https://link.springer.com/chapter/10.1007/978-3-319-53547-0_25)|[DSD100](https://sigsep.github.io/datasets/dsd100.html)|Spectrogram|*DeepConvSep* (CNN-based)|SAR, SDR, SIR, ISR|
|[Y. Luo, *et al.* (2017)](https://ieeexplore.ieee.org/abstract/document/7952118)|[DSD100-remix](https://sigsep.github.io/datasets/dsd100.html), iKala|Spectrogram|*Chimera*(Deep clustering, Bi-LSTM)|SDR|
|[S. Uhlich, *et al.* (2017)](https://ieeexplore.ieee.org/abstract/document/7952158)|[DSD100](https://sigsep.github.io/datasets/dsd100.html)|Spectrogram|*BLEND*(FNN(feed-forward) + Bi-LSTM)|SDR|
|[N. Takahashi and Y. Mitsufuji (2017)](https://ieeexplore.ieee.org/abstract/document/8169987)|[DSD100](https://sigsep.github.io/datasets/dsd100.html)|Spectrogram|*MM(Multiscale Multiband)DenseNet*|SDR|
|[D. Stoller, S. Ewert, and S. Dixon (2018)](https://arxiv.org/abs/1806.03185)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform|*Wave-U-Net*|SDR statistics|
|[S. Park, T. Kim, K. Lee, and N. Kwak (2018)](https://arxiv.org/abs/1805.08559)|[DSD100](https://sigsep.github.io/datasets/dsd100.html)|Spectrogram|Stacked Hourglass Network(CNN-based)|Median SDR|
|[J.Y. Liu and Y.H. Yang (2018)](https://ieeexplore.ieee.org/abstract/document/8614148)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html), [DSD100](https://sigsep.github.io/datasets/dsd100.html)|Spectrogram|ARC(Auto-encoder with Recurrent skip Connections) aka *Spect U-Net*|SDR|
|[N. Takahashi, N. Goswami, and Y. Mitsufuji (2018)](https://ieeexplore.ieee.org/abstract/document/8521383)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html), [DSD100](https://sigsep.github.io/datasets/dsd100.html)|Spectrogram|*MMDenseLSTM*|SDR|
|[F. Lluís, J. Pons, and X. Serra (2018)](https://arxiv.org/abs/1810.12187)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform|*Wave-Net*|SAR, SDR, SIR|
|[J.Y. Liu and Y.H. Yang (2019)](https://arxiv.org/abs/1906.01203)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|Dilated GRU|SDR|
|[F. Stöter, S. Uhlich, A. Liutkus, and Y. Mitsufuji (2019)](https://hal.inria.fr/hal-02293689/)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html), MUSDB18-HQ|Spectrogram|*Open-Unmix* (based on [S. Uhlich, *et al.* (2017)](https://ieeexplore.ieee.org/abstract/document/7952158))|SDR|
|[L. Prétet, *et al.* (2019)](https://ieeexplore.ieee.org/abstract/document/8683555)|*Bean* + [MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|U-Net|SAR, SDR, SIR|
|[Y. Luo and N. Mesgarani (2019)](https://ieeexplore.ieee.org/abstract/document/8707065)|WSJ0-2MIX (speech)|Waveform|Conv-TasNet|SI-SNR, SDR|
|[A. Défossez, *et al.*(2019)](https://arxiv.org/abs/1911.13254)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform|*Demucs*|SDR|
|[R. Hennequin, *et al.* (2020)](https://joss.theoj.org/papers/10.21105/joss.02154)|Train: *Bean* + Extra , Test: [MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|*Spleeter* (based on U-Net, [L. Prétet, *et al.* (2019)](https://ieeexplore.ieee.org/abstract/document/8683555))|SAR, SDR, SIR, ISR|
|[Y. Luo, *et al.* (2020)](https://ieeexplore.ieee.org/abstract/document/9054266)|WSJ0-2MIX (speech)|Spectrogram|DP(Dual-Path)RNN|SI-SNR, SDR|
|[E. Nachmani, Y. Adi, and L. Wolf (2020)](http://proceedings.mlr.press/v119/nachmani20a.html)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html), WSJ0-2MIX (speech)|Spectrogram|DPRNN-based|SDR|
|[D. Samuel and A. Ganeshan (2020)](https://ieeexplore.ieee.org/abstract/document/9053513)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform + Spectrogram|*Meta-TasNet* (meta-learning of ConvTasNet)|SI-SNR, SDR|
|[N. Takahashi and Y. Mitsufuji (2020)](https://arxiv.org/abs/2010.01733)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|*D3Net* (multidilated convolution)|SDR|
|[E. Lancaster, and N. Souviraà-Labastie (2020)](https://hal.science/hal-02986241/)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)+ Extra 30|Waveform|TasNet|SI-SNR, SDR|
|[W. Choi, *et al.* (2020)](https://arxiv.org/abs/2010.11631)|[MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|*LaSAFT-GPoCM* (Latent Source Attentive Frequency Transformation Gated Point-wise Convolutional Modulation)|SDR|
|[T. Li, *et al.* (2021)](https://ieeexplore.ieee.org/abstract/document/9362081)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|*Sams-Net* (Sliced Attention-based Neural Network)|SDR|
|[X. Song, *et al.* (2021)](https://arxiv.org/abs/2102.09966)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform + Spectrogram|*CatNet*|SDR|
|[Q. Kong, *et al.* (2021)](https://arxiv.org/abs/2109.05418)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|*ResUNet* (Residual UNet)|SDR|
|[R. Sawata, *et al.* (2021)](https://ieeexplore.ieee.org/abstract/document/9414044)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform + Spectrogram|*CrossNet-UnMiX (X-UMX)* (multi-domain loss, combination loss)|SDR|
|[H. Liu, Q. Kong, and J. Liu (2021)](https://arxiv.org/abs/2112.04685)|[MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|*CWS-PResUNet* (channel-wise subband phase-aware ResUNet), *ByteMSS* (CWS-PResUNet+DeMucs)|SDR|
|[A. Défossez (2021)](https://arxiv.org/abs/2111.03600)|[MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html)|Waveform + Spectrogram|Hybrid *Demucs*|nSDR|
|[M. Kim, *et al.* (2021)](https://arxiv.org/abs/2111.12203)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform + Spectrogram|*KUIELab-MDX-Net* (two-stream neural network)|SDR|
|[Y. Luo and J. Yu (2022)](https://arxiv.org/abs/2209.15174)|[MUSDB18, MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html)|Spectrogram|Band-Split RNN|uSDR, cSDR|
|[Y. Hu, *et al.* (2022)](https://ieeexplore.ieee.org/abstract/document/9812509)|[MUSDB18](https://sigsep.github.io/datasets/musdb.html)|Waveform + Spectrogram|*CDE-HTCN* (cross-domain encoder hierarchic temporal convolutional network)|SDR|

Papers in PDF available [here](https://github.com/jo-cho/music_source_separation_literatures/tree/main/MSS%20Literatures)

---
Explanation in Korean: [blog post](https://jo-cho.github.io/MIRBlog/posts/Experiments/Literatures_SS.html)
