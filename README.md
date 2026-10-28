# zml9167.github.io

这是一个 GitHub Pages 静态站点仓库，用于展示和游玩使用 **Godot 4** 开发的网页游戏。

首页 `index.html` 提供中英文双语界面，可查看游戏介绍、操作说明，并跳转到对应的游戏页面。

## 在线访问

- 游戏列表：[https://zml9167.github.io](https://zml9167.github.io)
- Snake：[https://zml9167.github.io/snake/Snake.html](https://zml9167.github.io/snake/Snake.html)
- Tetris：[https://zml9167.github.io/tetris/Tetris.html](https://zml9167.github.io/tetris/Tetris.html)

## 游戏列表

### Snake 游戏

- **描述**：经典贪吃蛇游戏，使用 Godot 4 开发，支持分数系统和渐进加速。
- **操作**：方向键（↑ ↓ ← →）或 WASD 控制移动。
- **玩法**：吃掉食物使蛇身变长并得分；撞到墙壁或自身身体则游戏结束。
- **源码**：[https://github.com/zml9167/snake](https://github.com/zml9167/snake)

### Tetris 游戏

- **描述**：经典俄罗斯方块游戏，使用 Godot 4.6 开发，支持等级进阶、最高分记录和存档功能。
- **操作**：方向键 / WASD 移动与旋转，`Q` 逆时针旋转，`Esc` 暂停；同时支持手柄操作。
- **玩法**：移动并旋转下落的方块，消除完整的水平行来得分；方块堆到顶部则游戏结束。
- **源码**：[https://github.com/zml9167/tetris](https://github.com/zml9167/tetris)

## 项目结构

```
.
├── index.html                  # 游戏列表首页（中英文切换、玩法弹窗）
├── README.md                   # 项目说明
├── .gitignore                  # Git 忽略规则（忽略 .vscode/）
│
├── snake/                      # Snake 游戏 Web 导出目录
│   ├── Snake.html              # 游戏入口页面（含 Godot 配置）
│   ├── Snake.js                # Godot Web 引擎加载脚本
│   ├── Snake.wasm              # WebAssembly 引擎（release，非多线程）
│   ├── Snake.pck               # 游戏资源包
│   ├── Snake.audio.worklet.js  # 音频工作线程脚本
│   ├── Snake.audio.position.worklet.js
│   ├── Snake.png               # 启动画面
│   ├── Snake.icon.png          # 页面图标
│   ├── Snake.apple-touch-icon.png
│   ├── README.md               # 游戏详细说明（英文）
│   └── README_zh.md            # 游戏详细说明（中文）
│
└── tetris/                     # Tetris 游戏 Web 导出目录
    ├── Tetris.html             # 游戏入口页面（含 Godot 配置）
    ├── Tetris.js               # Godot Web 引擎加载脚本
    ├── Tetris.wasm             # WebAssembly 引擎（release，非多线程）
    ├── Tetris.pck              # 游戏资源包
    ├── Tetris.audio.worklet.js # 音频工作线程脚本
    ├── Tetris.audio.position.worklet.js
    ├── Tetris.png              # 启动画面
    ├── Tetris.icon.png         # 页面图标
    ├── Tetris.apple-touch-icon.png
    ├── README.md               # 游戏详细说明（英文）
    └── README_zh.md            # 游戏详细说明（中文）
```

> 两个游戏均由 Godot 4.6 的 Web 导出模板构建（`template_release`、`nothreads`），因此 `Snake.wasm` 与 `Tetris.wasm` 内容一致，仅资源包不同。

## 如何访问

直接访问 [https://zml9167.github.io](https://zml9167.github.io)，在首页选择游戏即可开始游玩。

## 本地运行

由于游戏使用 WebAssembly 加载资源，需要通过 HTTP 服务访问，不能直接双击打开 HTML 文件。

1. 克隆本仓库到本地：
   ```bash
   git clone https://github.com/zml9167/zml9167.github.io.git
   cd zml9167.github.io
   ```
2. 启动本地静态服务器，例如使用 Python：
   ```bash
   python -m http.server 8000
   ```
3. 在浏览器中访问 `http://localhost:8000`。

## 更新游戏（重新导出）

1. 在 Godot 4.6 中打开对应游戏项目，使用 **Web** 导出预设重新导出。
2. 将新的 `.html`、`.js`、`.wasm`、`.pck` 以及图标、音频 worklet 等文件覆盖到 `snake/` 或 `tetris/` 目录。
3. 确认导出 HTML 中 `GODOT_CONFIG.fileSizes` 记录的 `.pck` / `.wasm` 文件大小与实际文件一致，否则加载进度和缓存校验可能异常。
4. 若引擎模板版本发生变化，请同步替换全部导出文件，避免 `.js`、`.wasm` 与 `.pck` 版本不匹配。
5. 提交前建议在本地服务器中实际运行一次，确认游戏可正常启动。

## 技术栈

- **游戏引擎**：Godot 4 / Godot 4.6（WebAssembly 导出，非多线程模式）
- **开发语言**：GDScript
- **前端页面**：原生 HTML / CSS / JavaScript，支持中英文切换
- **部署方式**：GitHub Pages 静态托管

## 未来计划

- 添加更多 Godot 小游戏
- 优化首页布局与移动端体验
- 增加游戏分类、搜索和标签功能

## 贡献

欢迎提交 Issue 或 Pull Request 来改进这个项目！
