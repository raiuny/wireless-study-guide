# 无线通信MAC层技术指南

## 目录

### 1. 媒体访问控制基础 (Media Access Control Fundamentals)
- [1.1 MAC层概述](./fundamentals/mac-overview.md)
  - MAC层功能
  - MAC层架构
  - MAC与PHY层接口
  - MAC与上层协议接口
- [1.2 帧结构与格式](./fundamentals/frame-structure.md)
  - 帧头设计
  - 帧尾设计
  - 数据帧格式
  - 控制帧格式
  - 管理帧格式

### 2. 接入控制机制 (Access Control Mechanisms)
- [2.1 竞争接入](./access-control/contention-based.md)
  - CSMA (Carrier Sense Multiple Access)
  - CSMA/CD (Collision Detection)
  - CSMA/CA (Collision Avoidance)
  - 二进制指数退避算法
  - 隐藏终端和暴露终端问题
- [2.2 预约接入](./access-control/reservation-based.md)
  - 轮询机制
  - 令牌环机制
  - 时隙预约
  - 带宽请求机制
- [2.3 混合接入](./access-control/hybrid.md)
  - PCF (Point Coordination Function)
  - HCF (Hybrid Coordination Function)
  - HCCA (HCF Controlled Channel Access)
  - EDCA (Enhanced Distributed Channel Access)

### 3. 调度算法 (Scheduling Algorithms)
- [3.1 基本调度算法](./scheduling/basic.md)
  - FIFO (First In First Out)
  - 轮转调度 (Round Robin)
  - 优先级调度
  - 最短作业优先
- [3.2 QoS调度算法](./scheduling/qos.md)
  - WFQ (Weighted Fair Queuing)
  - WRR (Weighted Round Robin)
  - DRR (Deficit Round Robin)
  - EDF (Earliest Deadline First)
  - GPS (Generalized Processor Sharing)
- [3.3 无线环境调度](./scheduling/wireless.md)
  - 信道感知调度
  - 多用户调度
  - 跨层调度
  - 机会调度

### 4. 错误控制与恢复 (Error Control and Recovery)
- [4.1 错误检测](./error-control/detection.md)
  - CRC (Cyclic Redundancy Check)
  - 校验和 (Checksum)
  - 海明码
  - 奇偶校验
- [4.2 自动重传请求](./error-control/arq.md)
  - Stop-and-Wait ARQ
  - Go-Back-N ARQ
  - Selective Repeat ARQ
  - 混合ARQ (HARQ)
- [4.3 前向纠错](./error-control/fec.md)
  - 卷积码
  - Reed-Solomon码
  - 涡轮码
  - LDPC码

### 5. 流量控制 (Flow Control)
- [5.1 端到端流量控制](./flow-control/end-to-end.md)
  - 滑动窗口协议
  - 停止等待协议
  - 拥塞窗口控制
- [5.2 链路层流量控制](./flow-control/link-layer.md)
  - 反压机制
  - 流量整形
  - 漏桶算法
  - 令牌桶算法
- [5.3 无线环境流量控制](./flow-control/wireless.md)
  - 信道自适应控制
  - 功率感知控制
  - 移动性感知控制

### 6. 拥塞控制 (Congestion Control)
- [6.1 拥塞检测](./congestion/detection.md)
  - 丢包检测
  - 延迟检测
  - 队列长度监测
  - 吞吐量监测
- [6.2 拥塞避免](./congestion/avoidance.md)
  - 主动队列管理
  - 早期随机丢弃
  - 显式拥塞通知
  - 负载均衡
- [6.3 拥塞控制算法](./congestion/algorithms.md)
  - TCP Vegas
  - TCP Westwood
  - TCP Cubic
  - BBR算法

### 7. 多信道管理 (Multi-Channel Management)
- [7.1 信道分配](./multi-channel/allocation.md)
  - 静态信道分配
  - 动态信道分配
  - 分布式信道分配
  - 集中式信道分配
- [7.2 信道协调](./multi-channel/coordination.md)
  - 信道切换协议
  - 信道状态信息交换
  - 信道质量评估
  - 信道预留机制
- [7.3 信道聚合](./multi-channel/aggregation.md)
  - 载波聚合
  - 信道绑定
  - 多信道MIMO
  - 认知信道聚合

### 8. 节能机制 (Energy Efficiency)
- [8.1 睡眠机制](./energy/sleep.md)
  - 周期性睡眠
  - 自适应睡眠
  - 协调睡眠
  - 深度睡眠
- [8.2 功率管理](./energy/power-management.md)
  - 动态功率调整
  - 功率感知路由
  - 节能调度
  - 能量收集感知
- [8.3 绿色MAC协议](./energy/green-mac.md)
  - 能效优化算法
  - 能耗建模
  - 性能与能耗权衡

### 9. 安全机制 (Security Mechanisms)
- [9.1 认证机制](./security/authentication.md)
  - 802.1X认证
  - WPA/WPA2/WPA3
  - 数字证书认证
  - 生物特征认证
- [9.2 加密机制](./security/encryption.md)
  - WEP加密
  - TKIP加密
  - AES加密
  - 端到端加密
- [9.3 访问控制](./security/access-control.md)
  - MAC地址过滤
  - 访问控制列表
  - 基于角色的访问控制
  - 动态访问控制

### 10. 移动性管理 (Mobility Management)
- [10.1 切换机制](./mobility/handoff.md)
  - 硬切换
  - 软切换
  - 垂直切换
  - 预测性切换
- [10.2 位置管理](./mobility/location.md)
  - 位置更新
  - 位置预测
  - 位置缓存
  - 分布式位置管理
- [10.3 移动性感知协议](./mobility/mobility-aware.md)
  - 快速BSS转换
  - 移动IP支持
  - 移动性感知路由
  - 位置感知调度

### 11. 跨层设计 (Cross-Layer Design)
- [11.1 PHY-MAC跨层](./cross-layer/phy-mac.md)
  - 链路自适应
  - 功率控制集成
  - 信道状态反馈
  - 联合优化
- [11.2 MAC-网络层跨层](./cross-layer/mac-network.md)
  - 路由感知MAC
  - QoS映射
  - 拥塞信息共享
  - 联合路由和调度
- [11.3 端到端跨层](./cross-layer/end-to-end.md)
  - 应用感知MAC
  - 服务质量保证
  - 资源预留
  - 性能监测

### 12. 特定应用MAC协议 (Application-Specific MAC)
- [12.1 传感器网络MAC](./applications/sensor-networks.md)
  - 低功耗MAC
  - 事件驱动MAC
  - 数据聚合MAC
  - 自组织MAC
- [12.2 车联网MAC](./applications/vehicular.md)
  - DSRC MAC
  - V2V通信MAC
  - V2I通信MAC
  - 高速移动MAC
- [12.3 物联网MAC](./applications/iot.md)
  - LPWAN MAC
  - 海量连接MAC
  - 异构网络MAC
  - 边缘计算MAC

## 标准协议

### IEEE 802系列
- [IEEE 802.11 Wi-Fi](./standards/802.11.md)
- [IEEE 802.15 个人局域网](./standards/802.15.md)
- [IEEE 802.16 WiMAX](./standards/802.16.md)
- [IEEE 802.22 认知无线电](./standards/802.22.md)

### 3GPP标准
- [LTE MAC](./standards/lte-mac.md)
- [5G NR MAC](./standards/5g-nr-mac.md)
- [NB-IoT MAC](./standards/nb-iot-mac.md)

### 其他标准
- [Bluetooth MAC](./standards/bluetooth.md)
- [ZigBee MAC](./standards/zigbee.md)
- [LoRaWAN MAC](./standards/lorawan.md)

## 参考资料

### 经典教材
- 《计算机网络》- Andrew S. Tanenbaum
- 《无线网络通信》- Andrea Goldsmith
- 《无线通信网络与系统》- William Stallings

### 标准文档
- IEEE 802.11标准系列
- 3GPP TS 36.321 (LTE MAC)
- 3GPP TS 38.321 (5G NR MAC)
- IEEE 802.15.4标准

### 学术期刊
- IEEE Transactions on Mobile Computing
- IEEE/ACM Transactions on Networking
- Computer Networks
- IEEE Network Magazine

### 会议论文集
- IEEE INFOCOM
- ACM MobiCom
- IEEE ICC
- IEEE GLOBECOM
