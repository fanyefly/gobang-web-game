# 🎮 五子棋完整版 - Gobang Web Game

一个功能完整的五子棋网页游戏，包含高亮显示、获胜提示、防卡死AI和静默约束系统。

## ✨ 核心功能

### 🎯 最后一个落子高亮
- **黑棋高亮**: 红色外圈 + 浅红内圈 + 白色中心点
- **白棋高亮**: 青色外圈 + 浅青内圈 + 黑色中心点
- **实时更新**: 每次落子后自动更新高亮
- **悔棋支持**: 悔棋后高亮正确更新到前一个棋子

### 🏆 获胜提示
- **胜利覆盖层**: 棋盘中央显示胜利信息
- **动画效果**: 弹出动画，视觉冲击力强
- **胜利连线**: 红色连线标记获胜的五子
- **平局提示**: 棋盘满时显示平局信息

### 🤖 防卡死AI
- **搜索限制**: 最多20个候选位置
- **超时控制**: 最多3秒思考时间
- **渐进加深**: 从深度1开始逐步加深
- **异常处理**: 出错时自动降级到简单AI

### 🔒 静默约束系统
- **棋子交替**: 黑→白→黑...
- **玩家交替**: 人类→AI→人类...
- **回合完成**: AI思考期间阻止玩家操作
- **无界面干扰**: 所有约束在后台静默执行

## 🎮 游戏模式

### 双人对战 (PVP)
- 两人轮流下棋
- 支持悔棋、重新开始、棋子交换

### 对战AI (5个难度级别)
1. **简单**: 随机下棋
2. **中等**: Minimax深度2
3. **困难**: Minimax深度3-优化
4. **专家**: Minimax深度4-优化
5. **大师**: Minimax深度5-优化

## 🚀 快速开始

### 在线体验
访问: [https://fanyefly.github.io/gobang-web-game/](https://fanyefly.github.io/gobang-web-game/)

### 本地运行
1. 克隆仓库:
   ```bash
   git clone https://github.com/fanyefly/gobang-web-game.git
   ```
2. 打开 `gobang-complete-final.html` 或 `index.html`

## 📁 文件说明

### 主要文件
- `gobang-complete-final.html` - **完整最终版** (推荐)
- `index.html` - 主页面
- `gobang-v2.2-optimized-ai.html` - 优化AI版本
- `gobang-v2.1-pro-ai.html` - 专业AI版本

### 测试文件
- `test-last-move-highlight.html` - 高亮效果测试
- `test-optimized-ai.html` - AI性能测试
- `complete-test-suite.html` - 完整测试套件

## 🛠️ 技术特性

### AI算法
- **Minimax算法** 配合 **Alpha-Beta剪枝**
- **候选位置优化** (最多20个位置)
- **迭代加深搜索** (从深度1开始)
- **超时控制** (最多3秒)

### 性能优化
- **棋盘缓存**: 棋盘背景只绘制一次
- **局部重绘**: 只绘制新棋子，棋盘保持不动
- **事件节流**: 防止快速点击导致的问题
- **内存管理**: 及时清理不需要的数据

### 用户体验
- **响应式设计**: 支持不同屏幕尺寸
- **键盘快捷键**: 支持键盘操作
- **状态保存**: 游戏状态自动保存
- **错误恢复**: 异常时自动恢复

## 📊 版本历史

### v2.2 (当前版本)
- ✅ 最后一个落子高亮显示
- ✅ 获胜提示覆盖层
- ✅ 防卡死AI优化
- ✅ 静默约束系统

### v2.1
- ✅ 专业AI算法 (Minimax深度3-5)
- ✅ 静默约束系统
- ✅ 性能监控

### v2.0
- ✅ 棋盘不刷新优化
- ✅ 真实五子棋AI算法
- ✅ 完整功能测试

### v1.0
- ✅ 基础五子棋功能
- ✅ 双人PVP模式
- ✅ AI对战模式

## 🔧 开发说明

### 项目结构
```
gobang-web-game/
├── gobang-complete-final.html    # 完整最终版
├── index.html                    # 主页面
├── README.md                     # 说明文档
├── style.css                     # 样式文件
├── game.js                       # 游戏逻辑
├── advanced-ai.js                # AI算法
├── test-*.html                   # 测试文件
└── version-1.1/                  # 历史版本
```

### 浏览器兼容性
- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+

## 📝 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🤝 贡献

欢迎提交Issue和Pull Request！

## 📞 联系

- GitHub: [@fanyefly](https://github.com/fanyefly)
- 项目地址: [https://github.com/fanyefly/gobang-web-game](https://github.com/fanyefly/gobang-web-game)

---

**🎮 立即开始游戏:** [https://fanyefly.github.io/gobang-web-game/](https://fanyefly.github.io/gobang-web-game/)