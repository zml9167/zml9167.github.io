# zml9167.github.io

这是一个GitHub静态页面仓库，用于展示和运行各种游戏。

## 游戏列表

### Snake 游戏
- **描述**：一个经典的贪吃蛇游戏，使用 Godot 引擎开发
- **运行方式**：点击[Snake 游戏](https://zml9167.github.io/snake/Snake.html)开始游玩

## 项目结构

```
├── index.html          # 游戏列表页面
├── README.md           # 项目说明文件
└── snake/              # Snake游戏目录
    ├── Snake.html      # 游戏主页面
    ├── Snake.js        # 游戏脚本
    ├── Snake.pck       # 游戏资源包
    ├── Snake.wasm      # WebAssembly文件
    └── 其他游戏相关文件
```

## 如何访问

直接访问 [https://zml9167.github.io](https://zml9167.github.io) 即可查看游戏列表并开始游玩。

## 本地运行

1. 克隆本仓库到本地
2. 进入仓库目录
3. 启动本地服务器（例如使用 Python）：
   ```bash
   python -m http.server 8000
   ```
4. 在浏览器中访问 `http://localhost:8000`

## 未来计划

- 添加更多游戏
- 优化页面设计
- 增加游戏分类功能

## 贡献

欢迎提交 Issue 或 Pull Request 来改进这个项目！