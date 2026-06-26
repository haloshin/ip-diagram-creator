# Assets

这个目录用于放公共发行版可分发的通用参考图和版式示例。

当前开源候选包只包含已确认可公开展示的示例图，不包含原始照片、主页截图、私有角色资产或不可分发参考图。

## 建议目录

```text
banner.webp
what-you-get-character-assets.webp
what-you-get-character-assets.png
what-you-get-diagram-modes.webp
what-you-get-diagram-modes.png

examples/
  gallery/
    workflow-overview-16x9.webp
    workflow-overview-16x9.png
    character-assets-sample.webp
    character-assets-sample.png
    article-illustration-low-density.webp
    article-illustration-low-density.png
    knowledge-card-high-density.webp
    knowledge-card-high-density.png
  ppt-mode/
    ppt-mode-gallery-8up.webp
    ppt-mode-gallery-8up.png
    ppt-mode-01-cover.webp
    ppt-mode-01-cover.png
    ...
  illustration-density/
    low-density.png
    mid-density.png
    high-density.png
  knowledge-cards/
    workflow-card.png
    comparison-card.png
    checklist-card.png
    framework-card.png
    diagnosis-card.png

templates/
  character-assets/
    character-main-anchor-example.png
    character-spec-board-example.png
    character-action-expression-small-scene-example.png
```

## 放置规则

- 只放你有权公开分发的参考图。
- `banner.webp` 是 README 首屏主视觉。
- `what-you-get-character-assets.webp` 是 README 的角色资产产出示例图，`what-you-get-character-assets.png` 是同图源文件。
- `what-you-get-diagram-modes.webp` 是 README 的图解产出示例图，`what-you-get-diagram-modes.png` 是同图源文件。
- `examples/gallery/` 放 README 可直接展示的最终成品图。
- gallery 里的 WebP 用于 README 展示，PNG 作为同图源文件保留。
- `examples/ppt-mode/` 放 PPT 演讲模式的公开样例图，包括 16:9 单页样例和 4 列 x 2 行 gallery。
- 低 / 中 / 高信息量参考图只服务手绘插图模式。
- 知识卡参考图按信息结构分类，不按信息量分类。
- 三张角色资产的示例版式可以放在 `templates/character-assets/`。
- 用户确认后的三张角色资产不要放进 Skill 包作为全局默认资产，应放到对应用户或项目输出目录。
- 从社媒平台、课程页面、设计网站或客户项目中看到的图，不要直接复制进仓库。
- README 展示图优先使用 WebP，保留 PNG 源文件即可。
