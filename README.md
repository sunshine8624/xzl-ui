## Useful Links
```xzl-ui/
├── apps/                        # 应用入口目录，包含实际的应用程序，如 Web 前端应用和 Docs（Storybook 实例）
│   ├── web/                     # 主应用：主应用程序的代码，如 Web 前端部分
│   │   ├── public/              # 静态资源目录，存放公共的静态文件，如图片、字体等
│   │   ├── src/                 # 源代码目录，包含 Web 应用的实际代码
│   │   │   ├── assets/          # 应用的静态资源文件夹，通常存放图片、CSS、字体等
│   │   │   ├── components/      # 组件目录，Web 应用的 UI 组件（例如按钮、输入框等）
│   │   │   ├── hooks/           # 自定义 React hooks 目录，存放一些自定义的 React 钩子
│   │   │   ├── pages/           # 页面目录，定义 Web 应用的页面组件
│   │   │   ├── services/        # 服务层目录，用于存放处理 API 请求或其他服务的代码
│   │   │   └── utils/           # 工具函数目录，用于存放通用的辅助函数
│   │   ├── .env                 # 环境变量配置文件，用于管理不同环境下的配置（如开发、生产
│   │   ├── .gitignore           # Git 忽略文件，指定 Git 应该忽略哪些文件和文件夹
│   │   ├── package.json         # `web` 应用的 `package.json` 文件，包含该应用的依赖和
│   │   ├── tsconfig.json        # `web` 应用的 TypeScript 配置文件，定义该应用的编译选项
│   │   └── webpack.config.js    # `web` 应用的 Webpack 配置文件，用于打包该应用
│   └── docs/                    # Storybook 实例：用于展示组件库的 Storybook 配置和实现
│       ├── public/              # 静态资源目录，存放公共的静态文件，如图片、字体等
│       ├── src/                 # 组件展示和故事定义源代码目录
│       │   ├── stories/         # 存放 Storybook 故事文件（UI 组件的展示）
│       │   ├── .storybook/      # Storybook 配置文件夹，存放 Storybook 的配置
│       │   ├── .env             # 环境变量配置文件，用于管理 Storybook 环境配置
│       │   ├── package.json     # `docs` 应用的 `package.json` 文件，包含 
│       │   ├── tsconfig.json    # `docs` 应用的 TypeScript 配置文件
│       └── package.json         # 根级别的 `docs` 项目配置文件
├── packages/                    # 所有共享包目录，包含共享的代码，如 UI 组件库和工具类库
│   ├── ui/                      # UI 组件库：定义和实现 UI 组件的包，供其他应用或项目使用
│   │   ├── src/                 # 组件库源代码目录，包含 UI 组件的实际实现
│   │   │   ├── components/      # UI 组件的实现，如按钮、输入框、卡片等组件
│   │   │   ├── hooks/           # 与 UI 组件相关的 hooks，存放一些自定义的 React 钩子函
│   │   │   └── utils/           # 组件库的工具类，通常是一些辅助的函数或类
│   │   ├── .storybook/          # Storybook 配置文件夹，存放组件库的 Storybook 配置
│   │   ├── package.json         # `ui` 组件库的 `package.json` 文件，定义组件库的依赖
│   │   ├── tsconfig.json        # `ui` 组件库的 TypeScript 配置文件
│   │   ├── jest.config.js       # Jest 配置文件，用于单元测试
│   │   ├── storybook.config.js  # Storybook 配置文件，用于定义 UI 组件在 Storybook 中
│   └── utils/                   # 通用工具函数：各种常用的工具函数集合，如格式化函数、
│       ├── src/                 # 工具函数源代码目录
│       │   ├── helpers/         # 各种辅助函数的实现
│       │   └── services/        # 通用服务函数（如 API 请求、数据处理等）
│       ├── package.json         # `utils` 工具包的 `package.json` 文件
│       └── tsconfig.json        # `utils` 工具包的 TypeScript 配置文件
├── .github/workflows/           # GitHub Actions 配置目录，用于 CI/CD 自动化工作流
│   ├── build.yml                # 构建工作流配置文件，定义如何自动构建项目
│   ├── deploy.yml               # 部署工作流配置文件，定义如何自动将项目部署到生产环境
│   └── test.yml                 # 测试工作流配置文件，定义如何自动运行测试
├── .changeset/                  # Changesets 变更记录目录
│   ├── config.json              # Changesets 配置文件，定义版本策略、发布方式等
│   ├── fine-colts-feel.md       # 自动生成的变更说明文件
├── turbo.json                   # Turborepo 配置文件，用于定义多个包的构建和开发流程
├── package.json                 # 根级别的 `package.json` 文件，包含根依赖，通常会定义
└── tsconfig.base.json           # TypeScript 基础配置文件，配置项目的 TypeScript 编译规则，通常会供多个子项目使用
```