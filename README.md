
# 🎮 Under Legend: Aetherium Ascension
## 传说之地：魔晶争霸 - 数字计分板
> 一款为《传说之地：魔晶争霸》桌游设计的数字计分工具，支持魔晶追踪、单位管理和胜利动画。
> 
[![GitHub Pages](https://img.shields.io/badge/demo-live-brightgreen)](https://sa1koro.github.io/DATT2300/)

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)


<img width="256" height="256" alt="image" src="https://github.com/user-attachments/assets/f68ea04c-33bd-47bf-8b59-43bd9c5e10e3" />

---

## 📖 游戏简介

《传说之地：魔晶争霸》是一款2-5人的策略对抗桌游，玩家扮演元素领主，通过占领矿井、收集魔晶和卡牌战斗，争夺重塑世界的力量。

**胜利条件**：第一个收集到 **42个或更多魔晶** 的玩家获胜！

---

## ✨ 功能特性

### 💎 魔晶追踪系统
- 实时记录魔晶数量，支持加减操作
- 达到42个魔晶时自动触发胜利动画
- 数据自动保存，刷新页面不丢失

### 🎲 单位管理系统
- 支持五种元素单位：
  - 🔥 火（默认2点生命值）
  - 💧 水（默认3点生命值）
  - ⚙️ 金（默认3点生命值）
  - 🌿 木（默认2点生命值）
  - 🪨 土（默认5点生命值）
- 单位血量可自由调整
- 一键删除已阵亡单位

### 👥 玩家管理
- 自定义玩家名称
- 玩家编号切换（1-5），便于多人游戏时识别顺序
- 单人独立计分模式，每位玩家可扫码独立使用

### 🎉 胜利动画
- 彩纸飘落特效
- 魔晶数字震动动画
- 全屏胜利提示

### 📱 移动端优化
- 响应式设计，完美适配手机屏幕
- 触摸优化，点击反馈流畅
- 支持二维码扫码访问

---

## 🚀 快速开始

### 在线使用
访问 GitHub Pages 部署的[在线版本](https://sa1koro.github.io/DATT2300/)



### 本地使用
1. 克隆仓库到本地

```
git clone https://github.com/Sa1koro/DATT2300.git
```

2. 在浏览器中打开 `index.html` 文件即可使用

---
## 📱 使用指南

### 基础操作
1. **修改玩家信息**：点击顶部文本框修改玩家名称
2. **切换编号**：点击 🔄 按钮循环切换玩家编号（1-5）
3. **调整魔晶**：使用 💎 两侧的 + / − 按钮增减魔晶数量

### 单位管理
1. **添加单位**：点击"添加单位"按钮，选择元素类型
2. **调整血量**：使用单位右侧的 + / − 按钮修改生命值
3. **删除单位**：点击单位最右侧的 × 按钮移除

### 游戏流程
1. **采集阶段**：根据控制的矿井数量手动增加魔晶（每个矿井+2）
2. **召唤单位**：在网页上添加对应元素的单位
3. **战斗阶段**：手动调整单位血量
4. **胜利判定**：魔晶达到42时自动触发胜利动画

---

## 🎯 游戏规则速查

### 元素克制关系
```
火 → 金 → 木 → 土 → 水 → 火 //克制攻击造成 **双倍伤害**
```

### 回合流程
1. **采集阶段**：控制的每个矿井生产2个魔晶[
2. **行动阶段**：
   - 免费执行1次"移动"或"抽卡"
   - 支付魔晶执行额外行动：
     - 移动：1魔晶
     - 抽卡：2魔晶
     - 召唤：根据卡牌费用
3. **结束阶段**：宣布回合结束

---

## 🛠️ 技术栈

- **前端框架**：纯 HTML5 + JavaScript (ES6+)
- **样式框架**：Tailwind CSS (CDN)
- **数据存储**：localStorage（浏览器本地存储）
- **部署平台**：GitHub Pages
---

## 📂 项目结构

```
.
 ├── index.html          # 主程序文件（单文件应用）
 ├── README.md           # 项目文档
 └── LICENSE             # 开源协议
```


---

## 🎨 界面预览

### 主界面
- 顶部：玩家名称与编号
- 中部：魔晶计数器（大号显示，易于查看）
- 下部：单位列表与管理按钮

### 胜利动画
- 全屏黑色遮罩
- 金色"胜利"文字脉动
- 彩色彩纸飘落特效

---

## 🔧 自定义配置

如需修改游戏参数，可编辑 `index.html` 中的以下常量：
```

// 元素类型与默认血量
 const ELEMENTS = [
 { emoji: '🔥', name: '火', defaultHP: 2 },
 { emoji: '💧', name: '水', defaultHP: 3 },
 { emoji: '⚙️', name: '金', defaultHP: 3 },
 { emoji: '🌿', name: '木', defaultHP: 2 },
 { emoji: '🪨', name: '土', defaultHP: 5 }
 ];

// 胜利所需魔晶数量
 const VICTORY_THRESHOLD = 42;

```
text

---

## 📋 待办事项

- [ ] 添加多语言支持（中文/英文切换）
- [ ] 实现游戏历史记录功能
- [ ] 增加音效开关
- [ ] 支持导出/导入游戏数据
- [ ] 添加暗黑/明亮主题切换

---

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建新分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 提交 Pull Request

---

## 📄 开源协议

本项目采用 MIT 协议开源，详见 [LICENSE](LICENSE) 文件。

---

## 👤 作者

**Huanrui Cao**

- GitHub: [@Sa1koro](https://github.com/Sa1koro)
- Email: kaminodice@gmail.com

---

## 🙏 致谢

- 游戏设计灵感来源于《聖剣伝説 LEGEND OF MANA》的世界观
- UI 框架：[Tailwind CSS](https://tailwindcss.com/)
- 托管平台：[GitHub Pages](https://pages.github.com/)

---

## 📸 截图


---

## 🎲 相关链接

- [完整游戏规则文档](./Rule_of_ULAA.md)
- [游戏设计博客](https://blog.saikoro.me)
- [反馈与建议](https://github.com/Sa1koro/DATT2300/issues)

---
