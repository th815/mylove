# 💕 My Love - 致亲爱的刘春迪

一个浪漫的表白网页，用代码记录我们的故事。

## ✨ 特性

- 🌸 **动态樱花树**：点击种子，看着爱情之树慢慢生长绽放
- 💌 **温馨情书**：打字机效果展示我们的故事
- ⏰ **爱情计时器**：实时显示在一起的每一天、每一小时
- 🎵 **背景音乐**：The Flood - 情感氛围满分
- 🎤 **歌词同步显示**：中英双语歌词随音乐滚动

## 🎬 在线预览

[点击访问](https://mylove.tianhao.tech/) *

## 📸 预览截图

![CleanShot 2025-10-03 at 17.27.42](https://fastly.jsdelivr.net/gh/th815/images//blogCleanShot%202025-10-03%20at%2017.27.42.png)

## 🚀 快速开始

### 本地运行

1. **克隆项目**
```bash
git clone https://github.com/th815/mylove.git
cd mylove
```

帮你写一个漂亮的 README.md 文件：

```markdown

```

2. **启动本地服务器**

使用 Python（推荐）：

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

或使用 Node.js：

```bash
npx http-server
```

3. **打开浏览器**

```
http://localhost:8000
```

### 部署到 GitHub Pages

1. 进入仓库 Settings
2. 找到 Pages 选项
3. Source 选择 `main` 分支
4. 点击 Save，等待部署完成

## 📁 项目结构

```
mylove/
├── index.html                        # 主页面
├── README.md                         # 说明文档
└── static/                           # 静态资源目录
    ├── TheFlood.mp3                  # 背景音乐
    ├── default.css                   # 样式文件
    ├── functions.js                  # 工具函数
    ├── love.js                       # 樱花树动画逻辑
    ├── jquery.min.js                 # jQuery 库
    ├── jscex.min.js                  # Jscex 核心库
    ├── jscex-parser.js               # Jscex 解析器
    ├── jscex-jit.js                  # Jscex JIT 编译器
    ├── jscex-builderbase.min.js      # Jscex 构建器基础
    ├── jscex-async.min.js            # Jscex 异步支持
    └── jscex-async-powerpack.min.js  # Jscex 异步增强包

```

## 🎨 自定义修改

### 修改情书内容

编辑 `index.html` 中的文字部分：

```html
<div id="code">
    <span class="say">亲爱的xxx，</span><br>
    <span class="say">我们的故事...</span><br>
    <!-- 修改这里的内容 -->
</div>
```

### 修改时间起点

在 `index.html` 中找到：

```javascript
var together = new Date();
together.setFullYear(2025, 7, 27);  // 年，月(0-11)，日
together.setHours(21);               // 小时
together.setMinutes(16);             // 分钟
```

### 更换背景音乐

1. 替换 `static/TheFlood.mp3` 为你的音乐文件
2. 修改歌词数组中的时间和文本

### 调整颜色

修改 CSS 中的颜色值：

```css
#code {
    color: #C85A8E;  /* 情书文字颜色 */
}

#lyric-en {
    color: #FFB6C1;  /* 英文歌词颜色 */
}

#lyric-cn {
    color: #FFD700;  /* 中文歌词颜色 */
}
```

## 🎵 歌词格式

歌词使用时间轴数组格式：

```javascript
const lyrics = [
    { time: 13.036, en: "英文歌词", cn: "中文翻译" },
    // 时间单位：秒
];
```

## 🌐 浏览器兼容性

- ✅ Chrome/Edge (推荐)
- ✅ Firefox
- ✅ Safari
- ⚠️ IE 不支持

## 💡 使用提示

1. **首次访问**：点击页面任意位置激活音乐播放（浏览器自动播放策略限制）
2. **最佳体验**：使用 Chrome 浏览器 + 耳机 🎧
3. **移动端**：已适配响应式布局，支持手机访问
4. **性能优化**：Canvas 动画已优化，流畅运行

## 📝 技术栈

- HTML5 Canvas - 绘制樱花树动画
- jQuery - DOM 操作
- Jscex - 异步动画流程控制
- CSS3 - 样式和动画效果
- Web Audio API - 音乐播放

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

如果这个项目对你有帮助，请给个 ⭐️ Star 支持一下~

## 📄 开源协议

[MIT License](LICENSE)

## 💖 致谢

- 感谢 Jscex 异步框架
- 感谢所有开源项目贡献者
- 灵感来源于经典的 JavaScript 表白网页

---

**用代码写下爱的诗篇** ❤️

*Made with ❤️ by 田昊*

