# 无线通信PHY层技术指南

## 目录

### 1. 调制技术 (Modulation Techniques)
- [1.1 基本调制技术](./modulation/basic-modulation.md)
  - ASK (Amplitude Shift Keying)
  - FSK (Frequency Shift Keying)
  - PSK (Phase Shift Keying)
  - QAM (Quadrature Amplitude Modulation)
- [1.2 高级调制技术](./modulation/advanced-modulation.md)
  - APSK (Amplitude Phase Shift Keying)
  - OFDM (Orthogonal Frequency Division Multiplexing)
  - FBMC (Filter Bank Multi-Carrier)
  - GFDM (Generalized Frequency Division Multiplexing)

### 2. 编码技术 (Coding Techniques)
- [2.1 信道编码](./coding/channel-coding.md)
  - 卷积码 (Convolutional Codes)
  - 块码 (Block Codes)
  - 涡轮码 (Turbo Codes)
  - LDPC码 (Low-Density Parity-Check Codes)
  - 极化码 (Polar Codes)
- [2.2 线路编码](./coding/line-coding.md)
  - NRZ (Non-Return-to-Zero)
  - Manchester编码
  - 差分编码
- [2.3 网络编码](./coding/network-coding.md)
  - 线性网络编码
  - 随机网络编码

### 3. 多址接入技术 (Multiple Access Techniques)
- [3.1 传统多址技术](./multiple-access/traditional.md)
  - FDMA (Frequency Division Multiple Access)
  - TDMA (Time Division Multiple Access)
  - CDMA (Code Division Multiple Access)
  - SDMA (Space Division Multiple Access)
- [3.2 新型多址技术](./multiple-access/advanced.md)
  - [OFDMA (Orthogonal Frequency Division Multiple Access)](./OFDMA.md)
  - SC-FDMA (Single Carrier FDMA)
  - NOMA (Non-Orthogonal Multiple Access)
  - RSMA (Rate-Splitting Multiple Access)

### 4. 天线技术 (Antenna Technologies)
- [4.1 天线基础](./antenna/basics.md)
  - 天线参数
  - 天线方向图
  - 天线增益
- [4.2 智能天线](./antenna/smart-antenna.md)
  - 自适应天线阵列
  - 波束成型 (Beamforming)
  - 波束赋零 (Null Steering)
- [4.3 MIMO技术](./antenna/mimo.md)
  - 2x2 MIMO
  - 大规模MIMO (Massive MIMO)
  - 毫米波MIMO
  - 智能反射面 (IRS)

### 5. 信道估计和均衡技术 (Channel Estimation and Equalization)
- [5.1 信道建模](./channel/modeling.md)
  - 多径衰落信道
  - 瑞利衰落
  - 莱斯衰落
  - 信道相关性
- [5.2 信道估计](./channel/estimation.md)
  - 导频辅助估计
  - 盲估计
  - 半盲估计
  - 压缩感知估计
- [5.3 均衡技术](./channel/equalization.md)
  - 线性均衡
  - 判决反馈均衡
  - 最大似然序列检测
  - 涡轮均衡

### 6. 同步技术 (Synchronization)
- [6.1 载波同步](./synchronization/carrier-sync.md)
  - 载波频率同步
  - 载波相位同步
  - 频偏估计与补偿
- [6.2 符号同步](./synchronization/symbol-sync.md)
  - 符号定时同步
  - 帧同步
  - 时偏估计与补偿
- [6.3 网络同步](./synchronization/network-sync.md)
  - 时钟同步
  - GPS同步
  - 网络时间协议

### 7. 功率控制技术 (Power Control)
- [7.1 发射功率控制](./power-control/transmission.md)
  - 开环功率控制
  - 闭环功率控制
  - 功率控制算法
- [7.2 功率分配](./power-control/allocation.md)
  - 注水算法
  - 凸优化方法
  - 机器学习方法

### 8. 频谱管理技术 (Spectrum Management)
- [8.1 频谱感知](./spectrum/sensing.md)
  - 能量检测
  - 特征检测
  - 匹配滤波检测
- [8.2 动态频谱接入](./spectrum/dynamic-access.md)
  - 认知无线电
  - 频谱共享
  - 干扰管理

### 9. 数字信号处理技术 (Digital Signal Processing)
- [9.1 滤波技术](./dsp/filtering.md)
  - FIR滤波器
  - IIR滤波器
  - 自适应滤波器
- [9.2 变换技术](./dsp/transforms.md)
  - 傅里叶变换
  - 小波变换
  - 离散余弦变换

### 10. 新兴技术 (Emerging Technologies)
- [10.1 毫米波通信](./emerging/mmwave.md)
  - 毫米波信道特性
  - 毫米波波束成型
  - 毫米波组网
- [10.2 太赫兹通信](./emerging/terahertz.md)
  - 太赫兹信道建模
  - 太赫兹天线设计
- [10.3 可见光通信](./emerging/vlc.md)
  - LED调制技术
  - 光学MIMO
- [10.4 量子通信](./emerging/quantum.md)
  - 量子纠缠
  - 量子密钥分发

## 参考资料

### 经典教材
- 《数字通信》- John G. Proakis
- 《无线通信原理与应用》- Theodore S. Rappaport
- 《现代数字和模拟通信系统》- B.P. Lathi

### 标准文档
- IEEE 802.11 (Wi-Fi)
- 3GPP LTE/5G NR
- IEEE 802.16 (WiMAX)

### 学术期刊
- IEEE Transactions on Communications
- IEEE Transactions on Wireless Communications
- IEEE Communications Magazine
