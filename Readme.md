# DrawYour47

一个前后端分离的项目，使用 Next.js 和 React 构建前端，Rust 和 Actix Web 构建后端。后端通过 Dify Workflow 集成 AI 画图功能，前端负责展示和交互。

## 技术栈

### 前端

- **框架**: Next.js
- **库**: React
- **包管理**: pnpm
- **样式**: CSS (可扩展为 Tailwind CSS 或其他)

### 后端

- **语言**: Rust
- **框架**: Actix Web
- **AI 集成**: Dify Workflow (用于 AI 画图)

## 项目结构

```text
DrawYour47/
├── frontend/          # 前端代码 (Next.js)
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
├── backend/           # 后端代码 (Rust)
│   ├── src/
│   ├── Cargo.toml
│   └── ...
└── README.md          # 项目说明
```

## 安装

### 前端安装

1. 进入前端目录：

   ```bash
   cd frontend
   ```

2. 安装依赖：

   ```bash
   pnpm install
   ```

### 后端安装

1. 进入后端目录：

   ```bash
   cd backend
   ```

2. 安装 Rust（如果尚未安装）：
   - 访问 [rustup.rs](https://rustup.rs/) 并按照说明安装。

3. 构建项目：

   ```bash
   cargo build
   ```

## 运行

### 运行前端

1. 进入前端目录：

   ```bash
   cd frontend
   ```

2. 启动开发服务器：

   ```bash
   pnpm dev
   ```

   前端将在 `http://localhost:3000` 运行。

### 运行后端

1. 进入后端目录：

   ```bash
   cd backend
   ```

2. 运行服务器：

   ```bash
   cargo run
   ```

   后端将在默认端口运行（通常是 8080 或根据配置）。

## 配置

### Dify Workflow 集成

后端通过 Dify Workflow 进行 AI 画图。请确保：

- 配置 Dify API 密钥和端点。
- 在 `backend/src/main.rs` 或配置文件中设置相关参数。

### 环境变量

创建 `.env` 文件在相应目录中，设置必要的环境变量，例如：

- 前端：API 端点
- 后端：数据库连接、Dify 配置等

## 功能

- **AI 画图**: 通过 Dify Workflow 生成图像。
- **前端展示**: 使用 React 和 Next.js 展示图像和交互界面。
- **前后端通信**: 通过 RESTful API 或 WebSocket 进行数据交换。

## 贡献

欢迎贡献！请遵循以下步骤：

1. Fork 本仓库。
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)。
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)。
4. 推送到分支 (`git push origin feature/AmazingFeature`)。
5. 打开 Pull Request。

## 许可证

本项目采用 MIT 许可证。详见 [LICENSE](LICENSE) 文件。

## 联系

如有问题，请通过 GitHub Issues 联系。
