# Find-Time-From-Videos
人工智能视觉识别视频中的时间显示

# Find Time From Videos

## 项目简介

`Find Time From Videos` 是一个用于从视频中提取时间信息的工具。该项目旨在通过分析视频帧中的时间戳或时间显示，自动识别并提取视频中的时间信息。这对于需要从视频中获取时间数据的用户非常有用，例如监控视频分析、时间戳提取等场景。

## 功能特性

- **时间戳识别**：自动识别视频帧中的时间戳或时间显示。
- **多格式支持**：支持多种时间格式的识别，包括但不限于 `HH:MM:SS`、`YYYY-MM-DD HH:MM:SS` 等。
- **视频处理**：支持处理多种视频格式，如 MP4、AVI、MKV 等。
- **批量处理**：支持批量处理多个视频文件，提高效率。
- **输出结果**：将提取的时间信息保存为文本文件或 CSV 文件，便于后续分析。

## 安装指南

### 依赖项

在运行本项目之前，请确保已安装以下依赖项：

- Python 3.6 或更高版本
- OpenCV
- Tesseract OCR
- FFmpeg

### 安装步骤

1. **克隆仓库**：

   ```bash
   git clone https://github.com/SCYtelils/Find-Time-From-Videos.git
   cd Find-Time-From-Videos
   ```

2. **安装 Python 依赖**：

   ```bash
   pip install -r requirements.txt
   ```

3. **安装 Tesseract OCR**：

   - **Ubuntu/Debian**:

     ```bash
     sudo apt-get install tesseract-ocr
     ```

   - **macOS**:

     ```bash
     brew install tesseract
     ```

   - **Windows**:

     请从 [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) 下载并安装。

4. **安装 FFmpeg**：

   - **Ubuntu/Debian**:

     ```bash
     sudo apt-get install ffmpeg
     ```

   - **macOS**:

     ```bash
     brew install ffmpeg
     ```

   - **Windows**:

     请从 [FFmpeg](https://ffmpeg.org/download.html) 下载并安装。

## 使用说明

### 命令行使用

1. **单个视频处理**：

   ```bash
   python find_time.py --input video.mp4 --output output.txt
   ```

2. **批量处理**：

   ```bash
   python find_time.py --input videos/ --output output.csv
   ```

### 参数说明

- `--input`：输入视频文件或文件夹路径。
- `--output`：输出文件路径，支持 `.txt` 或 `.csv` 格式。
- `--format`：时间格式（可选），默认为 `HH:MM:SS`。
- `--interval`：帧提取间隔（可选），默认为每秒提取一帧。

## 示例

假设你有一个视频文件 `example.mp4`，你可以使用以下命令提取时间信息：

```bash
python find_time.py --input example.mp4 --output time_info.txt
```

提取的时间信息将保存在 `time_info.txt` 文件中。

## 贡献指南

我们欢迎任何形式的贡献！如果你有改进建议或发现了问题，请提交 Issue 或 Pull Request。

1. **提交 Issue**：请在提交 Issue 时详细描述问题或建议。
2. **提交 Pull Request**：请在提交 Pull Request 时确保代码风格一致，并附带详细的描述。

## 许可证

本项目采用 MIT 许可证。详情请参阅 [LICENSE](LICENSE) 文件。

## 联系方式

如有任何问题或建议，请联系项目维护者：

- **Email**: [longzizhen2000@qq.com](mailto:longzizhen2000@qq.com)
- **GitHub**: [SCYtelils](https://github.com/SCYtelils)

---

感谢使用 `Find Time From Videos`！希望这个工具能为你的工作带来便利。
