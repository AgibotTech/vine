# ALOE 论文项目主页

本仓库是 ALOE 论文的配套项目主页，用于展示工作；论文将挂载于 arXiv，可在论文中放链接指向此页。

## 本地预览

在仓库根目录用任意静态服务器即可预览，例如：

```bash
# Python 3
python -m http.server 8000

# 或 npx
npx serve .
```

浏览器打开 `http://localhost:8000` 即可查看。

## 需要修改的内容

在 **`index.html`** 中按你的论文修改：

| 位置 | 说明 |
|------|------ |
| `<title>` | 页面标题，建议与论文标题一致 |
| `.paper-title` | 论文标题 |
| `.paper-subtitle` | 可选：一句话描述或副标题 |
| `.authors` | 作者列表，`href` 可改为个人主页/Google Scholar |
| `.affiliations` | 单位列表，与作者上标对应 |
| `.hero-figure img` | `src` 改为你的 teaser 图路径（可放 `images/teaser.png`） |
| `.caption` | 主图说明文字 |
| `.action-links` | **Paper (PDF)**、**Code**、**Video**、**Project Page** 的链接 |
| `.abstract p` | 论文摘要 |
| `.highlights ul` | 3–5 条亮点/贡献 |
| `.citation pre` | BibTeX 条目，便于他人引用 |

图片建议放在仓库内（如 `images/`），便于在 GitHub 上稳定访问。

## 在 GitHub 上发布（GitHub Pages）

1. 把本仓库 push 到你的 GitHub（例如 `username/paper-homepage`）。
2. 打开仓库 **Settings → Pages**。
3. **Source** 选 **Deploy from a branch**。
4. **Branch** 选 `main`（或你用的默认分支），**Folder** 选 **/ (root)**。
5. 保存后等一两分钟，页面地址为：
   - `https://<username>.github.io/<repo-name>/`

例如：`https://yourname.github.io/rss-paper/`。

## 在论文里放链接

在论文中写项目主页链接时，直接使用上面得到的 GitHub Pages 地址，例如：

> Project page: https://yourname.github.io/rss-paper/

或：**Code & project page**: [link](https://yourname.github.io/rss-paper/)。

## 文件结构

```
homepage/
├── index.html    # 主页面，需按论文内容修改
├── style.css     # 样式，可按需调整
├── README.md     # 本说明
└── images/       # 可选：放 teaser 等图片
```

修改完 `index.html` 和图片后，提交并 push 到 GitHub 即可更新在线主页。
