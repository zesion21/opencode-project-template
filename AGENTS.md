## 项目简介

卫星遥感数据处理系统是一个面向超低轨卫星的遥感影像处理平台，支持从原始数据到L1-L5级别产品的全流程自动化处理。系统采用前后端分离架构，前端使用Vue 3，后端使用Spring Boot。

## 技术栈

### 后端技术栈

- **框架**：Spring Boot 3.2.x
- **数据处理**：GDAL 3.x + Orekit 11.x
- **数据库**：PostgreSQL 15 + PostGIS
- **存储**：MinIO对象存储
- **任务调度**：Spring Batch 5.x
- **API文档**：SpringDoc OpenAPI 3

### 前端技术栈

- **框架**：Vue 3 + TypeScript + 选项式API
- **UI组件**：Antdv
- **地图引擎**：OpenLayers 7.x
- **状态管理**：Pinia
- **构建工具**：Vite

## 项目结构

```
/
├── README.md                    # 项目总览
├── docs/                        # 文档目录
│   ├── PRD.md                   # 产品需求文档
│   ├── ARCHITECTURE.md          # 系统架构设计
│   ├── API-SPEC.md              # API接口规范
│   └── CHANGELOG.md             # 变更日志
├── backend/                     # 后端
│   └── src/                     # 源代码
├── frontend/                    # Vue前端
│   ├── README.md                # 前端项目说明
│   ├── package.json             # 依赖配置
│   └── src/                     # 源代码
├── docker/                      # Docker配置
│   ├── docker-compose.yml       # 容器编排
│   ├── Dockerfile.backend       # 后端镜像
│   └── Dockerfile.frontend      # 前端镜像
└── scripts/                     # 脚本文件
    ├── init-db.sql              # 数据库初始化
    └── setup-env.sh             # 环境设置
```

## 技能调用

- 当进行需求分析时，请调用 @product 进行产品需求分析，生成的文档存储在 `docs/` 中。
<!-- - 当进行后台开发和API接口设计时，请调用 @backend ，并且只能读取和修改 `backend`目录下代码内容，生成的文档存储在 `docs/`，接口文档存储在 `docs/api.md` 中。 -->
- 当使用midway技术栈进行后台开发和API接口设计时，请调用 @backend-midway ，并且只能读取和修改 `backend`目录下代码内容，生成的文档存储在 `docs/`，接口文档存储在 `docs/api.md` 中。
- 当进行前端开发时，请调用 @frontend ，协同 @ui-ux-pro-max 进行页面设计， 并且只能读取和修改 `frontend`目录下代码内容， 生成的文档存储在 `docs/` 中。
- 当进行uniapp时，请调用 @uniapp-architect ，生成的文档存储在 `docs/` 中。
- 当开发Electron项目时，调用 @electron ，协同 @ui-ux-pro-max 进行页面设计，参考文档在`docs/`

## 行为与风格

- **语气**：专业、简洁，避免冗余。
- **行为**：
  1. 在编写代码前先确认需求细节。
  2. 输出带有简短解释的高质量代码。
  3. 必要时补充测试用例或调试建议。
- **责任范围**：
  - 从零构建大中小型应用（前后端皆可）
  - 调试和优化现有代码
  - 编写简短文档（如 README）

## 工具使用

- 优先调用 Web 搜索 MCP 获取最新技术信息
- 根据任务需要调用 GitHub MCP 获取示例或依赖
- 必要时调用 Deploy MCP 完成部署

## 特殊要求

- **代码质量**：
  - 遵循官方编码规范
  - 避免使用过期或不推荐的技术
- **文档编写**：
  - 所有文档采用 Markdown 格式
  - 包含必要的注释和说明
