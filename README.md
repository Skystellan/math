# 数学笔记与思维导图

本项目使用 Markdown 和 LaTeX 记录数学笔记，并通过 Markmap 生成思维导图结构。

## 项目结构

- **笔记文件 (.md):** 存放在各个主题文件夹中（例如 `algebra_notes.md`）。
- **思维导图源文件 (`mindmap_source.md`):** 定义了整个知识体系的层级结构，用于生成思维导图。
- **LaTeX 公式:** 笔记中通过 `$inline formula$` 和 `$$block formula$$` 嵌入数学公式。

## 如何使用

1.  **编写/编辑笔记:**
    - 使用 Markdown 语法。
    - 使用 LaTeX 语法编写数学公式。VS Code 推荐安装 `Markdown+Math` 或 `Markdown Preview Enhanced` 扩展以获得良好的预览效果。
2.  **更新思维导图:**
    - 编辑 `mindmap_source.md` 文件以反映笔记的结构。
    - 在 VS Code 中安装 `Markmap` 扩展。
    - 打开 `mindmap_source.md` 并使用 Markmap 扩展的命令生成或预览思维导图。
3.  **同步到 GitHub:**
    ```bash
    git add .
    git commit -m "你的提交信息"
    git push origin main
    ```

## 工具和扩展

- VS Code
- Git
- Markmap (VS Code 扩展)
- Markdown All in One (VS Code 扩展)
- Markdown+Math 或 Markdown Preview Enhanced (VS Code 扩展)

