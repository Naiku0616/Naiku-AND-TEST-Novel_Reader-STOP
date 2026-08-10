#  Novel Reader

支持多种个性化设置和阅读辅助功能。

![Flutter](https://img.shields.io/badge/Flutter-3.0%2B-blue?style=flat-square&logo=flutter)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Version](https://img.shields.io/badge/Version-1.0.0-blue?style=flat-square)

##  功能特性

###  阅读体验
 智能分页：自动将长文本分页显示，每页约1500字符
 流畅翻页：支持滑动手势翻页，动画流畅自然
 自动阅读：可调节速度的自动翻页模式（1-10速）
 书签管理：随时添加、删除书签，快速定位阅读位置
 阅读进度：自动保存阅读进度，支持断点续读
 
###  个性化设置
- **字体大小**：12px - 24px 自由调节
- **行距设置**：1.2 - 2.2 行高调节
- **字体选择**：系统默认、衬线体、等宽体、手写体四种字体
- **阅读主题**：
  -  日间模式（白色背景）
  -  夜间模式（深色背景）
  -  护眼模式（淡绿色背景）
  -  羊皮模式（暖色背景）

###  书架管理
- **文件导入**：支持从本地导入 TXT 格式小说文件
- **列表/网格视图**：自由切换书架展示方式
- **搜索功能**：支持按书名、作者搜索
- **高级筛选**：按阅读时间、添加时间、进度排序
- **阅读统计**：记录阅读时长、阅读页数等数据

##  快速开始

### 环境要求
- Flutter SDK >= 3.0.0
- Dart SDK >= 2.19.0
- Android SDK / iOS SDK / macOS / Windows / Linux

### 安装步骤

1. **克隆项目**
```bash
git clone https://github.com/yourusername/novel_reader.git
cd novel_reader
```

2. **安装依赖**
```bash
flutter pub get
```

3. **运行应用**
```bash
flutter run
```

### 构建发布

**Android APK**
```bash
flutter build apk --release
```

**iOS**
```bash
flutter build ios --release
```

**Windows**
```bash
flutter build windows --release
```

##  项目结构

```
novel_reader/
├── android/                    # Android 平台相关配置
├── ios/                        # iOS 平台相关配置
├── lib/                        # Flutter 源代码
│   ├── core/                   # 核心层
│   │   ├── services/           # 服务层
│   │   │   └── novel_importer.dart  # 小说导入服务
│   │   └── themes/             # 主题配置
│   │       └── app_theme.dart  # 应用主题定义
│   ├── data/                   # 数据层
│   │   ├── local/              # 本地存储
│   │   │   └── storage_service.dart # SharedPreferences 存储
│   │   └── models/             # 数据模型
│   │       ├── novel.dart           # 小说模型
│   │       ├── bookmark.dart        # 书签模型
│   │       ├── chapter.dart         # 章节模型
│   │       └── reading_stats.dart   # 阅读统计模型
│   ├── presentation/           # 表现层
│   │   ├── bloc/               # 状态管理
│   │   │   ├── novel_provider.dart  # 小说状态管理
│   │   │   └── theme_provider.dart  # 主题状态管理
│   │   ├── screens/            # 页面
│   │   │   ├── library_screen.dart  # 书架页面
│   │   │   └── reader_screen.dart   # 阅读页面
│   │   └── widgets/            # 组件
│   │       └── novel_card.dart      # 小说卡片组件
│   └── main.dart               # 应用入口
├── linux/                      # Linux 平台配置
├── macos/                      # macOS 平台配置
├── pubspec.yaml                # 依赖配置
└── README.md                   # 项目文档
```

##  技术栈

| 技术 | 用途 |
|------|------|
| **Flutter** | 跨平台 UI 框架 |
| **Provider** | 状态管理 |
| **SharedPreferences** | 本地数据持久化 |
| **File Picker** | 文件选择 |
| **UUID** | 唯一标识符生成 |
| **Google Fonts** | 字体支持 |

##  界面预览

### 书架页面
- 卡片式展示已导入的小说
- 显示书名、作者、阅读进度
- 支持长按快捷操作

### 阅读页面
- 顶部/底部菜单可隐藏
- 左侧/右侧/顶部/底部触控区域可配置
- 设置面板支持多种自定义选项

##  贡献指南

欢迎贡献代码！请遵循以下步骤：

1. Fork 本项目
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 发起 Pull Request

##  开源协议

本项目基于 MIT License 开源，详情请参阅 [LICENSE](LICENSE) 文件。

##  致谢

- [Flutter Team](https://flutter.dev/) - 优秀的跨平台框架
- [Flutter Packages](https://pub.dev/) - 丰富的插件生态

---

 如果本项目对您有帮助，欢迎给个 Star 支持一下！
