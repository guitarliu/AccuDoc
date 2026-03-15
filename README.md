## 📦 AccuDoc

**AccuDoc - 1:1 Precision Word Table Automation System**
> 一个无需后端、纯前端实现的 Word 表格 1:1 格式精准自动化填充系统。

---

### 🌟 项目简介 (Introduction)
**AccuDoc** 旨在解决办公自动化中“格式丢失”的终极痛点。它能够直接在浏览器中解析复杂的 Word 表格，允许用户通过可视化点击定义变量，并生成实时同步的填表界面。

与市面上大多数文档生成工具不同，AccuDoc 采用 **物理级 XML 原地替换技术**，确保导出的文档与原始模板在**字体、字号、颜色、对齐方式、单元格宽高**上保持 100% 的绝对一致。

---

### ✨ 核心特性 (Key Features)
- **1:1 格式保留**：通过深度克隆 Word 底层 `w:rPr` 和 `w:pPr` 属性，实现文字样式与段落对齐的完美复刻。
- **可视化定义**：无需编写代码或手动修改 Word 占位符。直接在网页预览图中“点哪填哪”，自动识别标签。
- **实时同步预览 (WYSIWYG)**：左侧表单输入，右侧文档即时反馈，字数溢出与排版效果一目了然。
- **智能焦点追踪**：点击输入框时，文档自动滚动并高亮对应单元格，彻底消除“不知道填哪”的困扰。
- **纯前端架构**：100% 浏览器端运行（PizZip + docxtemplater），无需服务器，保护数据隐私与安全。
- **默认值继承**：自动提取原表格内容作为填表初始值，极大减少重复录入工作。

---

### 🛠️ 技术栈 (Tech Stack)
- **Core**: Vanilla JavaScript (ES6+)
- **Libraries**: 
  - [PizZip](https://github.com/open-xml-templating/pizzip) - 内存级 Office 文档解压处理
  - [docxtemplater](https://github.com/open-xml-templating/docxtemplater) - Word 模板渲染引擎
  - [FileSaver.js](https://github.com/eligrey/FileSaver.js) - 客户端文件保存
- **Parsing**: DOMParser (XML 处理)

---

### 🚀 快速开始 (Quick Start)
1. 下载或克隆本项目。
2. 直接双击 `index.html`（或部署在 GitHub Pages）。
3. **开发者模式**：上传 Word 模板 -> 点击单元格标记变量 -> 完成设置。
4. **填表模式**：在左侧列表填入内容，实时观察右侧预览，最后点击“生成并下载”。

---

### 📌 为什么选择 AccuDoc?
传统的 Word 插件或库往往会破坏表格的原有排版（尤其是复杂的对齐和特殊的行业字体）。**AccuDoc** 的诞生就是为了让非技术人员也能轻松定义复杂的自动化表格，同时保证生成的成果物符合最严苛的行业公文格式要求。

---

### 📝 许可证 (License)
[MIT License](LICENSE)