# Snake 游戏

一个经典的贪吃蛇游戏，使用 Godot 4 引擎开发。

## 游戏介绍

这是一个经典贪吃蛇游戏的现代化实现，使用 Godot 4 引擎开发。游戏具有流畅的动画、响应式控制和现代化的界面设计。

## GitHub 仓库

游戏源代码托管在 GitHub：[https://github.com/zml9167/snake](https://github.com/zml9167/snake)

## 在线游玩

点击这里开始游戏：[Snake 游戏](https://zml9167.github.io/snake/Snake.html)

## 玩法说明

### 游戏目标
- 控制蛇移动，吃掉食物来增长身体
- 避免撞到墙壁或自己的身体
- 尽可能获得更高的分数

### 控制方式

**键盘控制：**
- **方向键（↑ ↓ ← →）**：控制蛇的移动方向
- **WASD 键**：替代方向键控制移动

### 游戏规则
1. 蛇会自动向前移动
2. 吃到食物后，蛇的身体会增长，分数增加
3. 撞到墙壁或自己的身体会导致游戏结束
4. 随着分数增加，游戏速度会逐渐加快

### 游戏特色
- 流畅的动画效果
- 响应式控制
- 分数系统
- 现代化界面设计
- 渐进式难度增加

## 技术栈

- **游戏引擎**：Godot 4
- **开发语言**：GDScript
- **图形**：2D 图形
- **部署**：WebAssembly (WASM)

## 项目结构

```
snake/
├── scene/
│   ├── food/          # 食物对象和逻辑
│   ├── hud/           # 游戏界面显示
│   ├── main/          # 主游戏场景和逻辑
│   └── snake/         # 蛇对象和逻辑
├── .editorconfig      # 编辑器配置
├── .gitattributes     # Git 属性
├── .gitignore         # Git 忽略规则
├── icon.svg           # 游戏图标
├── project.godot      # Godot 项目配置
└── README.md          # 说明文件
```

## 本地运行

1. 下载并安装 Godot 4
2. 克隆仓库：
   ```bash
   git clone https://github.com/zml9167/snake.git
   ```
3. 在 Godot 中打开项目（选择 `project.godot` 文件）
4. 点击播放按钮开始游戏

## 贡献

欢迎提交 Pull Request 来改进这个项目！

## 许可证

本项目采用 MIT 许可证 - 详情请查看 LICENSE 文件。
