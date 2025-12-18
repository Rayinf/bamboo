# Bangboo Factory (邦布工厂)

**Bangboo Factory** 是一个创意 Web 应用程序，利用 Google Gemini 3 Pro AI 的强大功能，将您的照片转化为定制的“邦布”角色，灵感来源于《绝区零》(Zenless Zone Zero) 的艺术风格。

只需上传任意照片，自定义心情和渲染风格，AI 就会将其重构为来自空洞的收藏级角色！

## ✨ 功能特性

- **图像转邦布**：将上传的照片转换为邦布风格的角色，同时保留关键特征。
- **自定义风格**：
  - **3D 赛璐珞风格 (3D Cel-Shaded)**：匹配《绝区零》的真实视觉风格，具有清晰的轮廓和鲜艳的色彩。
  - **扁平 2D 风格 (Flat 2D)**：干净的矢量艺术风格插图。
- **心情选择**：从各种表情（默认、开心、生气、悲伤等）中进行选择，赋予您的邦布独特的个性。
- **交互式 UI**：现代化的游戏风格界面，带有 CRT 叠加效果和流畅的动画。
- **Gemini 驱动**：利用先进的 `gemini-3-pro-image-preview` 模型生成高质量图像。

## 🖼️ 示例展示

<div align="center">
  <img src="screenshots/bangboo-1.png" width="200" alt="Bangboo Style 1" />
  <img src="screenshots/bangboo-2.png" width="200" alt="Bangboo Style 2" />
  <img src="screenshots/bangboo-3.png" width="200" alt="Bangboo Style 3" />
</div>

## 🛠️ 技术栈

- **前端**：React 19, TypeScript, Vite
- **样式**：Tailwind CSS
- **图标**：Lucide React
- **AI 集成**：Google GenAI SDK (`@google/genai`)

## 🚀 快速开始

按照以下步骤在本地设置项目。

### 前置要求

- Node.js (v18 或更高版本)
- npm 或 yarn
- 一个已启用 **Gemini API** 的 Google Cloud 项目。

### 安装步骤

1.  **克隆仓库**
    ```bash
    git clone https://github.com/Rayinf/bamboo.git
    cd bamboo
    ```

2.  **安装依赖**
    ```bash
    npm install
    ```

3.  **环境设置**
    在根目录创建一个 `.env` 文件，并添加您的 Google Gemini API 密钥：
    ```env
    # 注意：在 Vite 中进行客户端使用时，您可能需要特定配置
    # 或确保构建过程处理 process.env.API_KEY 替换。
    API_KEY=your_google_gemini_api_key_here
    ```
    *(注意：请确保您的 API 密钥安全，如果在客户端应用程序中使用，通常需要进行限制。)*

4.  **运行开发服务器**
    ```bash
    npm run dev
    ```

5.  **打开应用**
    访问 `http://localhost:5173`（或终端中显示的 URL）开始创建邦布！

## 📖 使用指南

1.  **上传图片**：拖放或选择一张照片到“输入数据 (Input Data)”区域。
2.  **配置**：
    - 选择 **心情 (Mood)**（例如：开心、生气）。
    - 选择 **渲染风格 (Render Style)**（3D 或 扁平）。
3.  **生成**：点击“生成邦布 (Generate Bangboo)”按钮。
4.  **保存**：生成完成后，您可以下载您的定制邦布图像。

## 🤝 贡献

欢迎贡献代码！请随意提交 Pull Request。

## 📄 许可证

本项目开源并遵循 [MIT 许可证](LICENSE)。

---
*免责声明：本项目为粉丝创作，与 HoYoverse 或《绝区零》无关。*
