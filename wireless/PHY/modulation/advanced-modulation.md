# 高级调制技术 (Advanced Modulation Techniques)

## APSK (Amplitude Phase Shift Keying) - 幅相移键控
- **原理**: 结合幅度和相位调制的优点
- **特点**: 在高阶调制中表现优异
- **应用**: 卫星通信、DVB-S2

## OFDM (Orthogonal Frequency Division Multiplexing) - 正交频分复用
- **原理**: 将高速数据流分成多个低速子载波
- **优点**: 
  - 抗多径衰落
  - 频谱效率高
  - 实现相对简单
- **缺点**: 对频偏敏感，峰均比高
- **应用**: Wi-Fi、LTE、DVB

## FBMC (Filter Bank Multi-Carrier) - 滤波器组多载波
- **原理**: 使用滤波器组代替循环前缀
- **优点**: 
  - 更好的频谱效率
  - 更低的带外泄漏
  - 更好的时频局部化
- **应用**: 5G候选技术

## GFDM (Generalized Frequency Division Multiplexing) - 广义频分复用
- **原理**: OFDM的推广形式，支持非正交子载波
- **优点**: 
  - 灵活的波形设计
  - 更低的带外辐射
  - 更好的时频局部化
- **应用**: 5G及未来通信系统

## 技术对比
| 技术 | 频谱效率 | 抗多径 | 实现复杂度 | 应用场景 |
|------|----------|--------|------------|----------|
| OFDM | 高 | 好 | 中 | 4G/Wi-Fi |
| FBMC | 很高 | 很好 | 高 | 5G研究 |
| GFDM | 很高 | 很好 | 高 | 未来通信 | 