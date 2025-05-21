# SEG-4X项目结构说明

### 本项目由以下三个独立的 Git 仓库组成，每个仓库承担不同的职责，用于分离项目主配置、通用框架与功能模块开发。
---

### 📁 主仓库：[`SEG-Project-4X-demo`](https://github.com/OSCAR-hi/SEG-Project-4X-demo)

- 本仓库为项目的主库，包含项目的整体结构、Unity全局项目设置、公共资源等内容；
- 不应包含任何具体的游戏功能模块。

---

### 📁 框架仓库：[`SEG-Framework`](https://github.com/OSCAR-hi/SEG-Framework)

- 此仓库为 Sleep Early Game 工作室的通用开发资源库；
- 主要用于存放可复用的开发工具、脚本组件和底层功能框架，方便未来在其他SEG的游戏项目中复用。

---

### 📁 模块仓库：[`SEG-Project-4X-demo-Modules`](https://github.com/OSCAR-hi/SEG-Project-4X-demo-Modules)

- 用于实际游戏功能模块的开发，是大家日常工作的主要部分；
- 每个功能模块请放入该仓库对应的文件夹下，保持结构清晰，避免模块间干扰。

---

### 📁 Excel配表仓库：[`SEG-Project-4X-demo-Excel-Configs`](https://github.com/OSCAR-hi/SEG-Project-4X-demo-Excel-Configs)

- 用于集中管理此项目中的Excel配置表，方便策划自主编辑参数调试和使用。

---

⚠️ **注意事项：**
- 请**勿直接修改** `SEG-Project-4X-demo` 与 `SEG-Framework` 仓库；
- 若确需改动，请**先与奥斯卡沟通确认**修改合理性；
- 经双方确认后，再向主库提交 Pull Request（PR） 进行合并。

---

## 提交信息规范

- 请在提交代码时遵循以下格式规范，以保证提交历史清晰、统一，便于协作和后续维护。

### 📌 格式要求

- 提交信息请用以下**规定前缀**之一开头：
  - `feat`：新增功能
  - `fix`：修复 bug
  - `chore`：项目杂务（如配置文件、构建流程、依赖等）
  - `refactor`：重构代码（不改变功能行为，优化结构或可读性）

- **前缀后紧跟英语输入法冒号和空格**  
  - `前缀: 描述内容`

- **前缀前不应有其他字符**（如 emoji、空格、换行等）

### ✅ 参考示例

```bash
feat: 新增尖刺方块实现
fix: 修复碰撞体检测判定
chore: 配置战斗数值表
refactor: 优化事件模块代码

