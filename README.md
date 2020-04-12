# A Benchmark Dataset for SSVEP-Based Brain-Computer Interfaces

> Wang Y, Chen X, Gao X, Gao S (2017) A benchmark dataset for SSVEP-based brain-computer interfaces. IEEE Transactions on Neural Systems and Rehabilitation Engineering 25:1746-1752.

原始数据下载地址：ftp://sccn.ucsd.edu/pub/ssvep_benchmark_dataset/
![实验范式](https://s1.ax1x.com/2020/04/12/GLiQAO.png)

## Participants

35个健康受试者（17名女性，平均年龄22岁），其中8人有SSVEP-based BCI的使用经验。见文档**Sub_info.txt**。

## Stimulus

40目标的BCI speller，刺激界面通过MATLAB Psychophysics Toolbox Version 3设计。40个刺激通过联合频相编码(JFPM)实现，刺激频率为8~15.8Hz，间隔0.2Hz，相位由0、0.5π、π和1.5π构成。参考**Freq_Phase.mat**。

## Experimental Design

数据是由离线cue-guided BCI实验采集的，分6个block，每个block包含40个trial，分别对应40个目标刺激。每个trial由0.5s target cue + 5s target stimuli + 0.5s screen blank构成，数据长度共6s。

## Data Acquisition

通过Synamps2 EEG system采集，64个通道（通道信息见**64-channels.loc**文件）；参考电极位于Cz，电导10KΩ以下；50Hz陷波；原始采样率为1000Hz，降采样到250Hz，故每个通道的数据长度为250*6。
