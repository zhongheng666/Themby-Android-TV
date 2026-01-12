因为Android TV端一直找不到好用的客户端，偶然看到说Yamby支持TV端了，结果发现其实只是能装，并没有对TV做适配。网上其他人的用着也不得劲，所以自己用AI搞了一个，放出来有需要的自己下载安装。

## ✨ 主要特性 (Features)

### 🎬 极致播放体验

- **智能播放策略**：
  - **智能转码拦截**：自动检测设备能力，对于设备不支持的格式（如部分设备不支持的 10-bit HEVC 或 HDR），自动请求服务端转码，防止黑屏或卡顿。
- **强大的内核**：基于 **Media3 (ExoPlayer)** 构建，播放稳定高效。
- **断点续播**：支持记录播放进度。进入详情页时，自动判断是否有历史记录，提供“继续播放”或“从头播放”选项。
- **FFmpeg拓展**：智能检测音频编码，不支持的编码启用ffmpeg软解，理论上可以解码包括DTS等的大部分音频格式，未验证，可能有BUG。

### 🎨 现代化 UI 设计

- **沉浸式详情页**：支持背景图淡入、背景音乐（Theme Songs）自动播放，营造影院级氛围。
- **优雅的播放器界面**：
  - 极简风格的控制条（OSD）。
  - **字幕优化**：告别传统的黑底字幕！采用无背景、带描边的 **高亮白字** 样式，观感更佳。
- **流畅交互**：基于 Compose 的丝滑动画，专为遥控器操作优化的焦点逻辑。

### 🛠️ 功能完备

- **~~多音轨/~~多字幕切换**：在播放器内快速切换字幕流。
- **画质调节**：支持切换码率（从 480P 到 原画）。
- **倍速播放**：支持 0.5x - 2.0x 倍速调节。
- **演职员浏览**：点击演员头像即可查看其相关作品。

## 📱 截图 (Screenshots)

| **首页 (Home)**          | **详情页 (Detail)**        |
| ------------------------ | -------------------------- |
| *(请在此处放置首页截图)* | *(请在此处放置详情页截图)* |

| **播放器 (Player)**          | **设置菜单 (Settings)**      |
| ---------------------------- | ---------------------------- |
| *(请在此处放置播放界面截图)* | *(请在此处放置播放设置截图)* |

## 🛠️ 技术栈 (Tech Stack)

本项目完全使用 **Kotlin** 编写，并采用了现代化的 Android 开发架构：

- **UI**: [Jetpack Compose for TV](https://www.google.com/search?q=https://developer.android.com/tv/compose) (Material3)
- **Language**: Kotlin
- **Dependency Injection**: [Hilt](https://www.google.com/search?q=https://dagger.dev/hilt/)
- **Video Player**: [Media3 / ExoPlayer](https://www.google.com/search?q=https://developer.android.com/media/media3)
- **Networking**: [OkHttp](https://www.google.com/search?q=https://square.github.io/okhttp/) + Coroutines
- **Image Loading**: [Coil](https://www.google.com/search?q=https://coil-kt.github.io/coil/)

## 📦 安装与使用 (Installation)

### 方式一：下载 APK

请前往 [Releases](https://www.google.com/search?q=../../releases) 页面下载最新的 `.apk` 安装包，并通过 U盘 或 ADB 安装到您的 Android TV / 电视盒子上。

### ~~方式二：自行编译~~ 暂无开放源代码打算

1. ~~克隆本项目到本地：~~
2. ~~使用 Android Studio (推荐 Ladybug 或更新版本) 打开项目。~~
3. ~~等待 Gradle Sync 完成。~~
4. ~~连接您的 Android TV 设备（开启 ADB 调试）。~~
5. ~~运行 `app` 模块。~~

## 📝 待办事项 (Roadmap)

- ~~[ ] 增加搜索功能~~
- ~~[ ] 支持直播电视 (Live TV)~~
- ~~[ ] 增加用户多账号快速切换~~
- ~~[ ] 音乐播放器模式~~
- 可能没有待办了，基本满足我个人使用了，发现bug了可能修一下

## ~~📄 许可证 (License)~~

~~本项目基于 MIT 许可证开源。详情请参阅 [LICENSE](https://www.google.com/search?q=LICENSE) 文件。~~

------

**Disclaimer**: Themby is an unofficial client and is not affiliated with Emby LLC.