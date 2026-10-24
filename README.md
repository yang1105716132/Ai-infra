# AI Infra、GPU 硬件与 Stanford CS336 综合学习项目

一套面向个人自学的 **36 周课程项目**，建议每周投入 10–12 小时。项目把 Stanford CS336 的语言模型实现课程与 GPU 硬件、分布式训练和 AI 基础设施结合起来，最终完成一个可复现的小型语言模型训练与推理系统。

## 从这里开始

1. 打开 [36 周课程大纲与逐周资料](docs/课程大纲与学习资料.md)，按周学习主题、CS336 讲座视频、论文/官方文档与实践交付物。
2. 在 [学习进度表](progress/学习进度.md) 中记录状态和每周产出。
3. 需要记录实验或复盘时，复制 [每周学习记录模板](templates/每周学习记录.md) 或 [实验记录模板](templates/实验记录.md)。
4. 进入 GPU 实验前，先在 CPU 上验证正确性；使用云 GPU 时记录设备、软件版本、时长和费用。

## 学习主线

- **CS336 与模型实现**：tokenizer、Transformer、训练、评测、数据处理、SFT/RLHF、RLVR 与多模态。
- **GPU 与性能**：加速器架构、内存层次、Roofline、CUDA/ROCm、Triton、kernel profiling。
- **AI Infra 与分布式**：节点和网络拓扑、NCCL/RCCL、DDP/FSDP/TP/PP、checkpoint、监控、推理服务与单位成本。
- **Capstone**：训练并部署一个小型语言模型，提交性能报告、容量与成本模型、复现说明和演示。

## 项目结构

```text
.
├── README.md
├── docs/
│   └── 课程大纲与学习资料.md
├── progress/
│   └── 学习进度.md
├── templates/
│   ├── 每周学习记录.md
│   └── 实验记录.md
├── outputs/
│   └── AI_Infrastructure_GPU_Hardware_学习项目.md  # 旧入口，指向 docs 正式文档
└── .gitignore
```

## 资源与复现约定

课程文档为每周涉及 CS336 的内容附上 Stanford Online 的讲座 YouTube 直链，并收录 Stanford 课程页面、讲义、作业、GPU 厂商文档、论文和工具文档。网页资源和软件版本可能更新，开始课程或实验时请以源站当前内容为准。

不要把原始语料、模型权重、checkpoint、访问令牌或云凭据提交到 Git。`.gitignore` 已排除常见的大型数据、模型和本地实验产物。

## 许可证

本仓库目前不声明开放许可证。收录的外部课程、论文、文档和视频仍归各自权利人所有；请遵循原站的访问、使用和引用规则。
