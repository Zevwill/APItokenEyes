# 📊 AI 额度监控器

一个纯本地运行的 HTML 页面，实时监控你的大模型 API 余额用量。

无需安装，无需服务器，下载 HTML 文件用浏览器打开即可使用。

![Windows](https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?logo=apple&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white)

---

## ✨ 功能特性

- 🔑 添加 API Key 即可自动识别平台并查询余额
- 🔄 每 60 秒自动刷新，支持手动刷新
- 📦 配置导入/导出，方便多设备迁移
- 🌐 支持 CORS 代理配置，兼容国内外平台
- 🏠 可作为桌面快捷方式 / 主屏幕图标使用

## 📋 支持平台

| 类型 | 平台 |
|------|------|
| **有余额查询** | DeepSeek / Moonshot (Kimi) / 硅基流动 / OpenRouter |
| **密钥验证** | OpenAI / Claude / 智谱GLM / 通义千问 / 百川 / 阶跃星辰 / MiniMax / 零一万物 / 字节豆包 / 小米MiMo / Groq / xAI / Mistral / Google Gemini |
| **自定义** | 任意 OpenAI 兼容中转站（new-api / one-api 等） |

## 🚀 快速开始

1. 下载 `用量监控.html` 文件
2. 用浏览器打开
3. 选择模型平台（或选"自动识别"）
4. 粘贴你的 API Key → 保存并校验
5. 完成，开始监控

## 📱 添加为快捷方式

### Windows

1. 将 `用量监控.html` 存放到固定位置（例如 `D:\Tools\`）
2. 右键文件 → **发送到** → **桌面快捷方式**
3. 双击即可用默认浏览器打开

> 💡 进阶：右键桌面 → 新建快捷方式，输入以下内容可获得无地址栏的独立窗口体验：
> ```
> "C:\Program Files\Google\Chrome\Application\chrome.exe" --app="D:\Tools\用量监控.html"
> ```

### iOS

1. 将 HTML 文件保存到 **"文件" App**（如 iCloud Drive 根目录）
2. 打开 **快捷指令 App** → 点击 **+** 新建
3. 添加以下操作：
   - **获取文件** → 选择 HTML 文件（关闭"每次询问"）
   - **以 Safari 打开**（或"快速查看"）
4. 点击顶部名称 → **添加到主屏幕**
5. 设置图标和名称 → 完成

### Android

1. 文件管理器找到 HTML 文件 → 用 **Chrome** 打开
2. 右上角 **⋮** → **添加到主屏幕**

> ⚠️ 如果 Chrome 未显示该选项（`file://` 协议限制），可安装
> [Shortcut Maker](https://play.google.com/store/apps/details?id=rk.android.app.shortcutmaker)
> 手动创建快捷方式，地址填写：
> ```
> file:///sdcard/Download/用量监控.html
> ```

## ⚠️ 注意事项

- **数据存储在浏览器本地**（localStorage），不同设备之间数据不互通
- 切换设备后需要通过 **设置 → 导出/导入配置** 迁移数据，或重新添加 Key
- 国外平台（OpenAI / Claude 等）可能受浏览器 CORS 策略限制，可在设置中配置代理前缀
- 所有 API Key 仅保存在本地，不会上传到任何服务器

## 📄 License

MIT
