# Single-encoder-dual-decoder
一个轻量级的多任务学习框架：采用ViT-S编码器提取共享特征，多分支解码器处理不同子任务，仅需单帧图像输入即可完成2D维度BEV视图生成。
<img width="900" height="600" alt="image" src="https://github.com/user-attachments/assets/6fdf4152-b59e-49e0-be70-9983e1d3b502" />



https://github.com/user-attachments/assets/c3c50ae2-6811-4ca3-b176-e13dd72b0d08





会在后续整理并补齐源码。

## 🙏 致谢 & 参考文献 (Acknowledgements & References)

本项目是对非结构化道路复杂环境感知的一次探索。本系统的顺利完成，离不开开源社区的伟大贡献。核心架构、预训练权重及部分任务分支的算法实现，深度参考并基于以下优秀的开源项目，特此向原作者团队致以最诚挚的感谢：

* **[Depth-Anything-V2](https://github.com/DepthAnything/Depth-Anything-V2)**: 本项目借鉴了其出色的基础模型架构，并使用了其预训练权重作为强大的特征提取主干网络（Encoder），为复杂的越野场景提供了极为鲁棒的几何与深度特征支持。
* **[offroad_roadseg](https://github.com/STLIFE97/offroad_roadseg)**: 本系统在构建越野道路语义分割分支（Decoder）以及相关数据预处理时，参考了该仓库的实现逻辑。
* **[Off-Road-Freespace-Detection](https://github.com/chaytonmin/Off-Road-Freespace-Detection)**: 本系统关于可通行区域（Freespace）检测分支的模型设计思路与评估方案，受到了该开源工作的极大启发。
