# 基本调制技术 (Basic Modulation Techniques)

## 概述
基本调制技术是无线通信中将数字信息转换为模拟信号的基础方法。

## ASK (Amplitude Shift Keying) - 幅移键控
- **原理**: 通过改变载波的幅度来表示数字信息
- **特点**: 实现简单，但抗噪声能力差
- **应用**: 早期数字通信系统

## FSK (Frequency Shift Keying) - 频移键控
- **原理**: 通过改变载波的频率来表示数字信息
- **特点**: 抗噪声性能较好，频谱效率一般
- **应用**: 低速数据传输

## PSK (Phase Shift Keying) - 相移键控
- **原理**: 通过改变载波的相位来表示数字信息
- **类型**: 
  - BPSK (Binary PSK)
  - QPSK (Quadrature PSK)
  - 8-PSK
- **特点**: 频谱效率高，抗噪声性能好

## QAM (Quadrature Amplitude Modulation) - 正交幅度调制
- **原理**: 同时改变载波的幅度和相位
- **类型**:
  - 16-QAM
  - 64-QAM
  - 256-QAM
- **特点**: 频谱效率很高，广泛应用于现代通信系统

## 性能比较
- **频谱效率**: QAM > PSK > FSK > ASK
- **抗噪声性能**: FSK > PSK > QAM > ASK
- **实现复杂度**: ASK < FSK < PSK < QAM 