# Pets

宠物领养数据分析与预测项目。基于马来西亚 PetFinder 平台数据，分析影响宠物被领养速度的关键因素，并构建预测模型。

## 项目结构

```
pets/
├── data/
│   ├── raw/                  # 原始数据
│   │   ├── train.csv         # 训练数据集
│   │   ├── BreedLabels.csv   # 品种标签（狗 240 种 + 猫 ~67 种）
│   │   ├── ColorLabels.csv   # 颜色标签（7 种）
│   │   └── state_labels.csv  # 马来西亚州属标签
│   └── processed/            # 处理后数据
├── notebook/                 # Jupyter Notebook 分析
├── src/                      # 源代码
├── report/                   # 报告输出
├── main.py                   # 入口脚本
├── pyproject.toml            # 项目依赖配置
└── README.md
```

## 技术栈

- **Python** >= 3.13
- **数据处理**: Pandas, NumPy
- **可视化**: Matplotlib, Seaborn
- **机器学习**: Scikit-learn
- **交互分析**: Jupyter Notebook
- **包管理**: uv

## 快速开始

### 1. 安装 uv（如未安装）

```bash
pip install uv
```

### 2. 创建虚拟环境并安装依赖

```bash
uv sync
```

### 3. 启动 Jupyter Notebook

```bash
uv run jupyter notebook
```

## 数据说明

数据来源于 PetFinder.my 宠物领养平台，包含以下主要特征：

| 特征 | 说明 |
|------|------|
| 品种 (Breed) | 240 种犬类 + 混合犬，约 67 种猫类 |
| 颜色 (Color) | 7 种毛色 |
| 州属 (State) | 马来西亚 16 个州/联邦直辖区 |
| 其他 | 年龄、体型、健康状况、照片数量等 |

## 许可

仅供学习与研究使用。
