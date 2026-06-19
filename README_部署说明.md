# GitHub Pages 部署说明

这个目录是统一经营分析入口的静态站点发布包。

## 上传内容

把本目录下所有文件和子目录完整上传到 GitHub 仓库根目录，或上传到仓库的 `docs/` 目录。

关键文件：

- `index.html`：GitHub Pages 默认首页，内容等同于统一经营分析入口。
- `统一经营分析入口_2026-06-18.html`：原始入口文件。
- `可视化工作台原型.html`：工作台详情页。
- `LTV_首贷月Cohort复购对比可视化_2026-01_obs_2026-06-18.html`：LTV by month 详情页。
- `data/manual_exports/...`：白名单、权责详情页。
- `.nojekyll`：禁用 Jekyll 处理，按静态文件原样发布。

## GitHub Pages 设置

在 GitHub 仓库中进入：

`Settings -> Pages -> Build and deployment`

如果文件放在仓库根目录：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/ (root)`

如果文件放在 `docs/`：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/docs`

保存后等待 GitHub Pages 构建完成，访问页面提示的 URL。

## 注意

GitHub Pages 页面通常是公网可访问的。这个报表包含经营数据，发布前请确认是否可以对外暴露。
