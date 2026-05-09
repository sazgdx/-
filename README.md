#智利植物识别系统
本项目是一个全面的植物识别系统，利用深度学习技术从图像中识别各种植物种类，并且引入了deepseek为用户科普和解答问题
## 目录结构

- `app/`
  - `config/`
    - `__init__.py`：初始化配置模块。
    - `config.py`：包含项目配置，如数据库连接、API密钥等。
  - `data/`
    - `test_images/`：用于验证的测试图像目录。
    - `train_images/`：用于训练模型的训练图像目录。
    - `test_labels.csv`：包含测试图像标签的CSV文件。
    - `train_labels.csv`：包含训练图像标签的CSV文件。
  - `model/`
    - `resnet_model.py`：实现用于植物识别的ResNet模型架构。
  - `model_train_predict/`
    - `predict.py`：使用训练好的模型进行预测的脚本。
    - `test_model.py`：测试模型性能的脚本。
    - `train.py`：训练植物识别模型的脚本。
  - `templates/`
    - `index.html`：Web界面的HTML模板，用于上传和识别植物图像。
  - `utils/`
    - `dataset.py`：用于加载和预处理数据集的实用函数。
    - `__init__.py`：初始化实用工具模块。
  - `save_models/`
    - `best_model.pth`：保存表现最佳的训练模型的目录。
  - `app.py`：处理Web请求并提供Web界面的主应用程序入口点。
  - `README.md`：项目文档和指南。
  - `requirements.txt`：运行项目所需的Python依赖列表。

## 使用方法

要使用植物识别系统，请按照以下步骤操作：

1. **设置环境**：创建虚拟环境并安装 `requirements.txt` 中列出的依赖项。

   ```bash
   pip install -r requirements.txt
