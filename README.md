当然，下面是为你的 **GitHub 图床仓库（如 `Blog-Image`）** 量身定制的 `README.md` 文件，含中英文双语，并重点说明你采用 CDN 的原因和图片访问方式：

---

## 📄 `README.md`：GitHub 图床仓库说明

```markdown
# Blog-Image 图床仓库（用于 Hexo 博客）

本仓库专用于存放 Hexo 博客中引用的图片资源，配合 [PicGo](https://github.com/Molunerfinn/PicGo) 实现一键上传、自动生成链接的图床方案。

## ✅ 使用方式

图片上传路径：`img/`

上传后建议使用 CDN 加速方式访问图片，格式如下：

```

[https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/your-image-name.png](https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/your-image-name.png)

````

> ✅ 注意：**不要使用 `raw.githubusercontent.com` 的 GitHub 原始链接**，该地址在国内加载慢甚至被墙，建议统一使用 jsDelivr CDN 加速。

## 🌐 图床使用示例

Markdown 引用方式：

```markdown
![](https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/example.png)
````

HTML 控制大小与位置示例：

```html
<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/example.png" width="60%">
</p>
```

## 📦 配置说明

* 图床工具：PicGo + GitHub 图床插件
* 上传方式：PicGo 自动上传至本仓库 `img/` 文件夹
* 渲染环境：Hexo 博客 / Markdown 编辑器（VSCode、Typora）

## ❗注意事项

* 本仓库应保持 **公开状态**，否则图片无法被外部访问
* 上传后如需更名或删除图片，请同步更新博客引用
* 不建议使用子分支、多层嵌套目录，避免链接复杂化

---

# Blog-Image: GitHub Image Hosting for Hexo Blog (via PicGo)

This repository is used as an image hosting service for my Hexo blog, powered by [PicGo](https://github.com/Molunerfinn/PicGo).

## ✅ How to Use

Uploaded images are placed in: `img/`

Access your image via CDN:

```
https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/your-image-name.png
```

> ⚠️ Do **not** use GitHub's `raw.githubusercontent.com` links — they are slow and often blocked in China. Use jsDelivr for best performance.

## 🌐 Example Usage

Markdown:

```markdown
![](https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/example.png)
```

With custom width:

```html
<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/BIT-Penry/Blog-Image@main/img/example.png" width="60%">
</p>
```

## 📦 Configuration Summary

* Uploader: PicGo + GitHub Plugin
* Storage Path: `img/`
* Blog Platform: Hexo (Static Blog Engine)

## ❗Notes

* This repository **must be public**
* After renaming or deleting images, update your blog references accordingly
* Prefer flat directory structure for simplicity

```
